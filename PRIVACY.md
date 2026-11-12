# Pandalytics — Politique de confidentialité / Privacy policy

> Brouillon à relire et compléter avant toute diffusion. Les champs `[…]` sont à remplir.
> Draft to review and complete before any distribution. Fields marked `[…]` must be filled in.

## Français

**Ce que fait l'application.** Pandalytics est une application de bureau Windows pour League of Legends. Elle affiche des statistiques de joueurs et de champions, aide pendant la sélection des champions et affiche un tableau des joueurs de la partie en cours.

**Données traitées.**
- Données de jeu fournies par l'API de Riot Games (identifiant de joueur « puuid », Riot ID, rang, historique de parties classées : champions, runes, objets, sorts d'invocation, pings, bans). Ces données concernent des joueurs de League of Legends, pas les utilisateurs de l'application en tant que tels.
- Données locales du client League of Legends sur l'ordinateur de l'utilisateur (compte connecté, phase de jeu, sélection de champion, données de la partie en cours), lues uniquement sur la machine et jamais envoyées ailleurs.
- Réglages de l'application (taille de l'interface, recherches récentes et favoris, dernier profil consulté), stockés dans le dossier `%APPDATA%\com.theo.lolcompanion\`.

**Stockage.** Une base SQLite locale (`pandalytics.db`) contient les parties classées publiques renvoyées par l'API Riot (données de match), utilisées pour calculer des statistiques agrégées. Ces données sont collectées par un serveur géré par l'auteur de l'application, puis copiées sur le PC à la demande de l'utilisateur. Durée de conservation : [à décider, par exemple 1 an, puis suppression]. Sauvegardes : [à préciser].

**Ce que l'application ne fait pas.** Pas de compte utilisateur, pas de publicité, pas de suivi de l'usage, pas de revente de données, pas de collecte de données personnelles sur les utilisateurs de l'application. Aucun envoi de données du client League of Legends vers un serveur.

**Connexions réseau.** API de Riot Games (avec la clé de l'application, qui reste en local dans `config.json` et n'est jamais affichée ni journalisée), Data Dragon (icônes et noms), et, si l'utilisateur lance la synchronisation, le serveur de collecte de l'auteur (connexion chiffrée, l'application y télécharge une copie de la base et n'y envoie aucune donnée de joueur).

**Journal.** L'application écrit un journal technique local (`pandalytics.log`, erreurs et messages techniques, sans clé). Il n'est jamais envoyé.

**Contact et suppression.** theo.buchon3@gmail.com. Pour supprimer les données locales : désinstaller l'application et supprimer le dossier `%APPDATA%\com.theo.lolcompanion\`.

## English

**What the app does.** Pandalytics is a Windows desktop app for League of Legends. It shows player and champion statistics, assists during champion select, and shows a table of the players in the current game.

**Data processed.**
- Game data provided by the Riot Games API (player identifier "puuid", Riot ID, rank, ranked match history: champions, runes, items, summoner spells, pings, bans). This data concerns League of Legends players, not the app's users as such.
- Local League client data on the user's own computer (signed-in account, game phase, champion select, live game data), read on the machine only and never sent elsewhere.
- App settings (interface size, recent searches and favorites, last viewed profile), stored in `%APPDATA%\com.theo.lolcompanion\`.

**Storage.** A local SQLite database (`pandalytics.db`) holds public ranked matches returned by the Riot API (match data), used to compute aggregated statistics. This data is collected by a server run by the app's author, then copied to the PC when the user starts a sync. Retention period: [to be decided, e.g. 1 year, then deletion]. Backups: [to be specified].

**What the app does not do.** No user accounts, no advertising, no usage tracking, no resale of data, no collection of personal data about the app's users. No League client data is sent to any server.

**Network connections.** Riot Games API (with the application's key, which stays local in `config.json` and is never displayed or logged), Data Dragon (icons and names), and, when the user starts a sync, the collection server run by the author (encrypted connection; the app downloads a copy of the database and sends no player data to it).

**Log.** The app writes a local technical log (`pandalytics.log`, errors and technical messages, no keys). It is never uploaded.

**Contact and deletion.** theo.buchon3@gmail.com. To delete local data: uninstall the app and delete `%APPDATA%\com.theo.lolcompanion\`.

## Riot Games notice

Pandalytics isn't endorsed by Riot Games and doesn't reflect the views or opinions of Riot Games or anyone officially involved in producing or managing Riot Games properties. Riot Games, and all associated properties are trademarks or registered trademarks of Riot Games, Inc.
