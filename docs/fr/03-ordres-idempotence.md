# 03 — Ordres, annulations et idempotence

`ExchangeClient` regroupe placement, modification et annulation des ordres.
Une réponse réseau ambiguë ne dit pas toujours si l’action a été acceptée côté chaîne.
Renvoyer aveuglément un ordre peut alors créer une intention économique supplémentaire.
Le client doit rapprocher identifiants, état utilisateur et événements avant de réessayer.
Les identifiants fournis par le client facilitent le suivi d’une intention à travers les réponses.
L’annulation doit distinguer ordre absent, déjà exécuté et réellement annulé.
Les limites de précision et de taille appartiennent aussi à la validation préalable.
L’idempotence est ici une propriété applicative critique, pas seulement une optimisation réseau.

Suite : [WebSocket et cohérence](04-websocket-coherence.md).
