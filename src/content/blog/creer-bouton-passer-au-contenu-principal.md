---
title: 'Comment créer un bouton « Passer au contenu principal »'
description: 'Lorem ipsum dolor sit amet'
pubDate: 'Dec 05 2023'
heroImage: '/blog-placeholder-4.jpg'
---

Sur la majorité des sites accessibles, lorsqu'un utilisateur appuie sur la touche <kbd>TAB</kbd> en arrivant sur la page, un lien pour sauter directement au contenu principal est proposé.

![Bouton « Passer directement au contenu principal » sur Google](/projet-ergonomie/skip-to-main-content-google.png)

Voici comment mettre cela en place sur votre propre site. Tout d'abord ajouter un **id** sur votre contenu principal ainsi qu'un lien y menant au début de votre page, par exemple :

```html
<!doctype html>
<html lang="en">
	<head>
	</head>
	<body>
		<a href="#main" class="skip-to-main-content">Passer au contenu principal</a>
		<!-- VOTRE HEADER, NAVIGATION, ETC -->
		<main id="main">
            <!-- VOTRE CONTENU PRINCIPAL -->
        </main>
    </body>
</html>
```

Ensuite, il suffit de masquer le lien en CSS sauf si il est focus (grâce à la touche <kbd>TAB</kbd>). Il est conseillé de mettre un fond de couleur si vous avez un contenu tel qu'un logo en dessous.

```css
.skip-to-main-content {
	position: absolute;
	left: -9999px;
	background: #fff;
	padding: 1rem;
}

.skip-to-main-content:focus {
	left: 0;
}
```