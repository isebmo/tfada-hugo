---
title: Problème de lenteur film 4K depuis votre NAS
description: Résolvez vos problèmes de lenteurs lors du streaming de films 4K depuis votre NAS Synology
tags: 
author: iSebmo
date: 2019-12-02
categories: 
- Geek
- Applications
fimg: https://tfada.s3-eu-central-1.amazonaws.com/2019/lenteur-4k-synology.jpeg
---

Si comme moi vous constatez des problèmes de lenteur en visionnant vos films 4K depuis votre NAS je vous conseille d'aller voir du côté du protocole SMB. 
En effet le partage de fichier sur samba semble plus lent qu’en simple ftp. Sur mon [synology](https://www.amazon.fr/s?k=synology&__mk_fr_FR=%C3%85M%C3%85%C5%BD%C3%95%C3%91&ref=nb_sb_noss_2) j'ai simplement activé le partage au travers du protocole ftp et depuis je peux lire les films 4K sur infuse sur mon [Apple TV 4K](https://www.amazon.fr/APPLE-CPU-ACCESSORIES-MQD22FD-0190198463784/dp/B075LW3J5B/ref=sr_1_2?__mk_fr_FR=%C3%85M%C3%85%C5%BD%C3%95%C3%91&keywords=Apple+TV+4K&qid=1575228397&sr=8-2). 

J'ai aussi remarqué qu’[Infuse Pro](https://firecore.com/infuse) n'était pas optimisé pour la lecture de vidéos en 4K. En revanche je vous invite à essayer [Plex](https://www.plex.tv/fr/) qui à la différence de Infuse vous oblige à installer la partie serveur sur un NAS ou un ordinateur type raspberry. Mais [Plex](https://www.plex.tv/fr/) est capable de diffuser sans problème un flux 4K sans coupure. 
Je ferai un dossier sur ce logiciel que je trouve extraordinaire. 

Voilà si vous pensez être dans le même cas de figure je vous conseille de faire le changement. 
Profitez-en pour changer le port par défaut de FTP pour éviter de vous faire pirater un peu trop facilement. 

Bon film 🎥 !