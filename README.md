# Gemini Test Prospection - Radar 50 km (Calcul Réel des Coordonnées)

Application commerciale de prospection locale pour vendre des sites web aux artisans et commerçants dans un rayon strict de 50 km.

## Correctifs appliqués
- **Élimination de l'anomalie « Paris à 33 km »** :
  - Remplacement de la règle de repli par défaut qui réassignait arbitrairement les coordonnées de Rennes aux villes non reconnues.
  - Résolution réelle des coordonnées de Paris (~350 km de Médréac), excluant automatiquement ces sièges parisiens du rayon de 50 km.
  - Exclusion automatique des sièges sociaux parisiens et hors-département lors des scans SIRENE pour ne conserver que les artisans locaux.
- **Ajout des artisans de l'Ouest d'Ille-et-Vilaine** : Intégration directe des artisans situés autour de Médréac (35360), Montauban-de-Bretagne, Bédée, Saint-Méen-le-Grand et Montfort-sur-Meu.
- **Clarification du bouton Réinitialiser** : Indication explicite de réinitialisation vers Ercé-près-Liffré sans confusion avec la commune sélectionnée.
