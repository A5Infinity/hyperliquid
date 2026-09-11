# 02 — Signatures et séparation de domaine

Les actions de trading sont sérialisées avant d’être signées par le portefeuille.
Une représentation canonique est indispensable : deux encodages différents produisent deux signatures différentes.
Le domaine de signature lie l’intention au protocole et au type d’action attendu.
Chaîne, adresse, nonce et payload doivent être vérifiés avant toute demande au portefeuille.
Le SDK propose des helpers, mais l’interface reste responsable d’expliquer ce qui sera signé.
Une signature ne doit jamais être recyclée sur un autre environnement ou une autre action.
Les changements de sérialisation sont donc des modifications de sécurité et de compatibilité.
La revue doit suivre les données depuis l’objet typé jusqu’aux octets effectivement signés.

Suite : [ordres et idempotence](03-ordres-idempotence.md).
