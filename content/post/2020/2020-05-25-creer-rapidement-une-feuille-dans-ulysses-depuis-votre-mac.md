---
title: Créer rapidement une feuille dans Ulysses depuis votre mac
description: 
tags: 
- productivité
author: iSebmo
date: 2020-05-25
categories: 
- LifeHack
- Applications
fimg: https://tfada.s3-eu-central-1.amazonaws.com/ulysses-2020.jpg
---

Si vous utilisez Ulysses sous Mac afin de gérer vos posts de blog ou vos essais, ou tout simplement pour gérer vos idées vous vous demandez surement comment rapidement les noter dans l’application sans avoir à l’ouvrir. 
Quand j’ai une idée, il faut que je l’écrive immédiatement sans quoi je risque de l’oublier 😝 . C’est pourquoi, je me suis mis à la recherche d’un équivalent de ce que je fais avec l’application Raccourcis sur iOS afin d’écrire l’idée rapidement et que la feuille se crée dans Ulysses.

Vous n’avez pas vraiment besoin de savoir développer pour le faire, mais les lignes de code ne doivent pas vous effrayer non plus. 
D’abord vous allez lancer l’éditeur de scripts sous Mac. Recopiez les lignes suivantes dans un nouveau fichier de script :

	set theResponse to display dialog "Idée de post ?" default answer "" with icon note buttons {"Cancel", "Continue"} default button "Continue"
	
	if button returned of theResponse is "Continue" then
		open location "ulysses://x-callback-url/new-sheet?text=" & (text returned of theResponse)
	end if

Ensuite il faut créer une application depuis ce script, pour cela je vous ai facilité la tâche avec ce GIF :

![](https://tfada.s3-eu-central-1.amazonaws.com/new-sheet-ulysses-2.gif)

À présent que votre application est prête, il suffit de la rechercher à l’aide de Spotlight :

![](https://tfada.s3-eu-central-1.amazonaws.com/new-sheet-ulysses-1.gif)

Je vous laisse l’adresse de la documentation technique des x-call-back d’Ulysses afin de modifier le script comme bon vous semble.

J’espère que vous n’oublierez plus rien grâce à cette astuce 😽.
