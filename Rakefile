require "rubygems"
require "tmpdir"
require "bundler/setup"
require "jekyll"
require 'json'

# Indiquez le nom de votre dépôt
GITHUB_REPONAME = "guillaumew/simbios"
ENV["JEKYLL_ENV"] = "production"

namespace :site do
  desc "test"
  task :test do
    sh "alias ecoindex-cli=\"docker run -it --rm --add-host=host.docker.internal:host-gateway -v /tmp/ecoindex-cli:/tmp/ecoindex-cli vvatelot/ecoindex-cli:latest ecoindex-cli\""
    sh "ecoindex-cli analyze --url https://simbios.fr --recursive --export-format json"
  end

  desc "Calcul des ecoindex des pages publiées"
  task :ecoindex do 
    ARGV.each { |a| task a.to_sym do ; end }
    file_path = "/tmp/ecoindex-cli/output/simbios.fr/#{ARGV[1]}/results.json"
    if(File.exist?(file_path)) then
      f = File.read(file_path)
      ecoscores = JSON.parse(f)
      output = ""
      ecoscores.each { |row|
        path = row['url'][18..-1]
        output = "#{output}- path: #{path}\n  score: #{row['score']}\n  grade: #{row['grade']}\n  size: #{row['size'].round}\n  nodes: #{row['nodes']}\n  requests: #{row['requests']}\n"
      }
      File.write('_data/ecoindex.yml', output)
      puts "Ecodindexes successfully updated"
    else
      puts "File not found"
    end
  end

  desc "Génération des fichiers du site"
  task :generate do
    Jekyll::Site.new(Jekyll.configuration({
      "source"      => ".",
      "destination" => "_site"
    })).process
  end

  desc "Génération et publication des fichiers sur GitHub"
  task :publish => [:generate] do
    Dir.mktmpdir do |tmp|
      cp_r "_site/.", tmp
      
      pwd = Dir.pwd
      Dir.chdir tmp
      File.open(".nojekyll", "wb") { |f| f.puts("Site généré localement.") }
      
      system "git init"
      system "git add ."
      message = "Site mis à jour le #{Time.now.utc}"
      system "git commit -m #{message.inspect}"
      system "git remote add origin git@github.com:#{GITHUB_REPONAME}.git"
      system "git push origin master:refs/heads/gh-pages --force"

      Dir.chdir pwd
    end
  end
end