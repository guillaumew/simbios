---
title: "Minifier les ressources javascript, CSS et HTML"
description: Voici un des dix commandements pour diminuer rapidement l'empreinte environnementale d'un site internet.
tags: ["Site", "Eco-conception", "CSS", "Javascript", "HTML"]
image: /assets/img/posts/2024/Q1/ecoconception-site.webp
thumb: /assets/img/posts/2024/Q1/ecoconception-site
hidden: true
---

## Le problème 

Dans le code, il y a de nombreux caractères que l'on écrit mais qui servent uniquement pour une meilleure compréhension de ce que fait le code :
- commentaires
- sauts de ligne
- indentations
- noms de variables compréhensibles

Il est totalement justifié de conserver ces caractères lorsque l'on modifie le code, mais par contre, ces derniers totalement inutiles pour le bon fonctionnement du site.

Il convient donc de les retirer au moment où l'on sert les fichiers de code (Javascript, CSS, HTML et SVG). C'est ce qu'on appelle la minification.

Exemple de gains de taille :

| Fichier            | Taille non minifié | Taille minifié | Gain   |
|--------------------|--------------------|----------------|--------|
| Bootstrap (CSS)    | 169.5 ko           | 137.6 ko       | -18.8% |
| Bootstrap JS       | 120.9 ko           | 49.8 ko        | -58.8% |
| HTML ce cette page | 10.1 ko            | 8.7 ko         | -13.9% |

## Comment faire ?

Il existe de nombreux outils. Certains en ligne prennent le code et le minifient. D'autres, plus pratiques, se greffent dans le projet pour minifier les ressources lors du build du site.

Quelques exemples :

- Javascript
  - {% include link.html link="https://minify-js.com/" text="Minify JS" %} (online)
  - {% include link.html link="https://extendsclass.com/javascript-formatter.html" text="ExtendsClass" %} (online)
  - {% include link.html link="https://www.npmjs.com/package/uglify-js" text="UglifyJS" %} (in build)
- CSS
  - {% include link.html link="https://www.cleancss.com/css-minify/" text="Clean CSS" %} (online)
  - {% include link.html link="https://cssnano.github.io/cssnano/" text="CSSNano" %} (in build)
- HTML
  - {% include link.html link="https://codebeautify.org/minify-html" text="HTML Minifier" %} (online)
  - {% include link.html link="https://www.npmjs.com/package/htmlnano" text="htmlnano" %} (in build)
- SVG
  - {% include link.html link="https://svgomg.net/" text="SVGOMG" %} (online)
  - {% include link.html link="https://svgo.dev/" text="SVGO" %} (in build)

## Ensuite ?

- Voir le commandement suivant : [Les fichiers, tu compresseras](08-compresser-fichiers.html)
- [Revenir à la liste de commandements](dix-min-pour-reduire-empreinte-environnementale-site.html)
