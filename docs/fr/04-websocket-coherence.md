# 04 — WebSocket, reconnexion et cohérence

Les abonnements diffusent des mises à jour après une photographie initiale ou un état déjà connu.
Une coupure peut créer un intervalle pendant lequel des événements ne sont pas observés.
La reconnexion doit restaurer les abonnements sans les dupliquer.
Après reprise, une lecture HTTP permet de réconcilier la vue locale avec l’état canonique.
Les consommateurs doivent tolérer messages répétés et changements arrivant dans un ordre inattendu.
Un curseur temporel seul ne suffit pas toujours à ordonner des événements concurrents.
Les gestionnaires doivent être retirés lorsque l’écran ou la stratégie cesse de les utiliser.
Cette discipline évite fuites, doubles traitements et décisions fondées sur un carnet périmé.

Suite : [HyperEVM et limites](05-hyperevm-limites.md).
