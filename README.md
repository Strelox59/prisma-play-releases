<p align="center">
  <img src="icon-1.png" width="128" alt="Logo Prisma Play">
</p>

<h1 align="center">Prisma Play</h1>

<p align="center">
  Lecteur IPTV pour Windows et macOS : TV en direct, films, séries et sport, dans une interface pensée pour le canapé.
</p>

<p align="center">
  <a href="https://github.com/Strelox59/prisma-play-releases/releases/latest"><b>⬇️ Télécharger la dernière version</b></a>
</p>

---

Ce dépôt contient uniquement les **installateurs** de Prisma Play. Le code source est privé.

> **Prisma Play ne fournit aucune chaîne ni aucun contenu.** C'est un lecteur : tu y ajoutes ta propre playlist (Xtream Codes ou M3U) fournie par ton abonnement IPTV.

## Fonctionnalités

- **TV en direct** : guide des programmes, listes de chaînes personnalisées, retour en arrière et pause sur le direct (jusqu'à 1 h).
- **Films et séries** : affiches, notes, bandes-annonces, reprise de la lecture, épisode suivant automatique, badge « Nouvel épisode » sur les séries suivies.
- **Sport** : matchs en direct et à venir (football, NBA, NFL, rugby, tennis, F1…), chaîne qui diffuse le match trouvée automatiquement, rappels avant le coup d'envoi, score sur l'icône de la barre des tâches ou du Dock.
- **Lecteur** : image dans l'image, sous-titres personnalisables, vitesse de lecture, minuterie de mise en veille, passage du générique.
- **Personnalisation** : couleurs, fonds, polices et taille de l'interface ; le logo suit la couleur choisie.
- **Mises à jour automatiques** : l'app te prévient quand une nouvelle version est disponible et s'installe toute seule.

## Installation

### Windows

1. Télécharge **`Prisma.Play.Setup.x.x.x.exe`** dans la [dernière version](https://github.com/Strelox59/prisma-play-releases/releases/latest).
2. Lance-le. Windows peut afficher « Windows a protégé votre ordinateur », car l'app n'est pas signée : clique sur **Informations complémentaires**, puis **Exécuter quand même**.
3. Suis l'installation.

### macOS

1. Télécharge le zip qui correspond à ton Mac :
   - **`PrismaPlay-x.x.x-macOS-AppleSilicon.zip`** pour les Mac M1, M2, M3, M4 et plus récents ;
   - **`PrismaPlay-x.x.x-macOS-Intel.zip`** pour les Mac Intel plus anciens.
2. Double-clique sur le zip, puis glisse **Prisma Play** dans le dossier **Applications**.
3. L'app n'étant pas signée par Apple, ouvre le **Terminal** et colle cette commande pour la débloquer :

   ```
   chmod -R u+w "/Applications/Prisma Play.app" && xattr -cr "/Applications/Prisma Play.app" && codesign --force --deep -s - "/Applications/Prisma Play.app" && open "/Applications/Prisma Play.app"
   ```

   Le message « replacing existing signature » est normal. Si le Terminal répond « Operation not permitted », active **Terminal** dans Réglages Système › Confidentialité et sécurité › **Gestion des apps**, puis recommence.

Cette étape n'est à faire qu'une fois : les versions suivantes s'installent automatiquement.

## Mises à jour

Prisma Play vérifie régulièrement ce dépôt. Quand une nouvelle version est publiée, un bouton **Mettre à jour** apparaît : l'app télécharge la nouvelle version, l'installe et se relance. Tu peux aussi vérifier à la main dans **Réglages › Diagnostic › Rechercher une nouvelle version**.

Tes playlists, favoris, historique et réglages sont conservés.

## Confidentialité

Tout reste sur ton ordinateur : tes playlists, identifiants et historique ne sont envoyés nulle part. L'app contacte seulement ton fournisseur IPTV, ainsi que des services publics pour enrichir l'affichage : affiches et notes de films, résultats sportifs, bandes-annonces et vérification des mises à jour sur ce dépôt.

## Configuration requise

- Windows 10 ou 11 (64 bits)
- macOS 11 Big Sur ou plus récent (Apple Silicon ou Intel)
