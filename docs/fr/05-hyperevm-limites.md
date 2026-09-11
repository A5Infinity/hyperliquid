# 05 — HyperEVM, finalisation et limites

Le SDK expose des actions liées à HyperEVM, notamment la modification d’utilisateur EVM et la finalisation de contrat.
Ces opérations relient des intentions signées au contexte EVM de l’écosystème Hyperliquid.
L’intégrateur doit distinguer adresse EVM, compte de trading et réseau sélectionné.
Une transaction EVM confirmée et un état de trading observé peuvent avoir des temporalités différentes.
Les interfaces doivent présenter explicitement cette attente et éviter d’annoncer une finalité prématurée.
Ce parcours couvre transports, signatures, ordres, reconnexion et points d’intégration HyperEVM.
Il ne constitue ni audit du protocole ni conseil de trading, et le SDK demeure communautaire.
Aucune installation, compilation ou exécution n’a été effectuée ; les tests et exemples amont restent les références de validation.
