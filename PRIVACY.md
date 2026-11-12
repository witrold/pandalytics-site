# Pandalytics — Politique de confidentialité / Privacy policy

> Brouillon à relire et compléter avant toute diffusion. Les champs `[…]` sont à remplir.
> Draft to review and complete before any distribution. Fields marked `[…]` must be filled in.

## Français

**Ce que fait l'application.** Pandalytics est une application de bureau Windows pour League of Legends. Elle affiche des statistiques de joueurs et de champions, aide pendant la sélection des champions et affiche un tableau des joueurs de la partie en cours.

**Données traitées.**
- Données de jeu fournies par l'API de Riot Games (identifiant de joueur « puuid », Riot ID, rang, historique de parties classées : champions, runes, objets, sorts d'invocation, pings, bans). Ces données concernent des joueurs de League of Legends, pas les utilisateurs de l'application en tant que tels.
- Données locales du client League of Legends sur l'ordinateur de l'utilisateur (compte connecté, phase de jeu, sélection de champion, données de la partie en cours), lues uniquement sur la machine et jamais envoyées ailleurs.
- Réglages de l'application (taille de l'interface, recherches récentes et favoris, dernier profil consulté), stockés dans le dossier `%APPDATA%\com.theo.lolcompanion\`.

**Stockage.** Une base SQLite sur le serveur de l'auteur contient les parties classées publiques renvoyées par l'API Riot (données de match), utilisées pour calculer des statistiques agrégées. Ces données sont collectées et stockées sur un serveur géré par l'auteur de l'application ; elles ne sont pas copiées sur le PC de l'utilisateur, qui ne reçoit que des statistiques calculées. Durée de conservation : 1 an, puis suppression. Sauvegardes : [à préciser].

**Ce que l'application ne fait pas.** Pas de compte utilisateur, pas de publicité, pas de suivi de l'usage, pas de revente de données, pas de collecte de données personnelles sur les utilisateurs de l'application. Aucun envoi de données du client League of Legends vers un serveur.

**Connexions réseau.** Le serveur de l'auteur (connexion chiffrée, authentifiée par un jeton personnel). L'application lui envoie le Riot ID recherché ou le Riot ID du joueur connecté pour afficher un profil, la partie en cours ou des statistiques ; le serveur interroge l'API de Riot Games avec sa propre clé, qui n'est jamais dans l'application ni affichée ni journalisée. Le serveur ne conserve pas ces requêtes au-delà des journaux techniques [durée à préciser]. L'application contacte aussi Data Dragon (icônes et noms).

**Journal.** L'application écrit un journal technique local (`pandalytics.log`, erreurs et messages techniques, sans clé). Il n'est jamais envoyé.

**Contact et suppression.** theo.buchon3@gmail.com. Pour supprimer les données locales : désinstaller l'application et supprimer le dossier `%APPDATA%\com.theo.lolcompanion\`.

## English

**What the app does.** Pandalytics is a Windows desktop app for League of Legends. It shows player and champion statistics, assists during champion select, and shows a table of the players in the current game.

**Data processed.**
- Game data provided by the Riot Games API (player identifier "puuid", Riot ID, rank, ranked match history: champions, runes, items, summoner spells, pings, bans). This data concerns League of Legends players, not the app's users as such.
- Local League client data on the user's own computer (signed-in account, game phase, champion select, live game data), read on the machine only and never sent elsewhere.
- App settings (interface size, recent searches and favorites, last viewed profile), stored in `%APPDATA%\com.theo.lolcompanion\`.

**Storage.** A SQLite database on the author's server holds public ranked matches returned by the Riot API (match data), used to compute aggregated statistics. This data is collected and stored on a server run by the app's author; it is not copied to the user's PC, which only receives computed statistics. Retention period: 1 year, then deletion. Backups: [to be specified].

**What the app does not do.** No user accounts, no advertising, no usage tracking, no resale of data, no collection of personal data about the app's users. No League client data is sent to any server.

**Network connections.** The author's server (encrypted connection, authenticated with a personal token). The app sends it the Riot ID being looked up, or the connected player's Riot ID, to show a profile, the current game or statistics; the server queries the Riot Games API with its own key, which is never in the app and never displayed or logged. The server does not keep these requests beyond technical logs [retention to be specified]. The app also contacts Data Dragon (icons and names).

**Log.** The app writes a local technical log (`pandalytics.log`, errors and technical messages, no keys). It is never uploaded.

**Contact and deletion.** theo.buchon3@gmail.com. To delete local data: uninstall the app and delete `%APPDATA%\com.theo.lolcompanion\`.

## Riot Games notice

Pandalytics isn't endorsed by Riot Games and doesn't reflect the views or opinions of Riot Games or anyone officially involved in producing or managing Riot Games properties. Riot Games, and all associated properties are trademarks or registered trademarks of Riot Games, Inc.
