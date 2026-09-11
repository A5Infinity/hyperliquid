# 01 — Un SDK typé sur deux transports

Ce dépôt communautaire expose l’API Hyperliquid aux principaux environnements JavaScript.
Les clients séparent les requêtes HTTP des abonnements WebSocket persistants.
Les types TypeScript rendent visibles paramètres et réponses attendus avant l’exécution.
Le transport HTTP convient aux lectures ponctuelles et aux actions signées.
Le WebSocket sert les flux de marché, d’ordres et d’état utilisateur.
Une application doit prévoir déconnexion, reconnexion et messages reçus hors ordre.
Le typage réduit certaines erreurs d’intégration sans garantir la fraîcheur des données réseau.
Le SDK doit être identifié comme communautaire, et non comme une bibliothèque officielle Hyperliquid.

Suite : [signatures et domaine](02-signatures-domaine.md).
