# validation-sncf-transilien

La mobilité des voyageurs peut être appréhendée avec les données de validations, c’est-à-dire à partir des informations relatives au passage d’une carte ou d’un ticket à un valideur (date, heure, nature, lieu, etc.). Deux types de valideurs co-existent :

- Les CAB, qui constituent une ligne fermée à franchir en validant pour accéder au quai. Ils permettent de remonter les validations télébilletiques et magnétiques. Il existe deux types de CAB :
	- Sur les CAB tripode ancienne génération (G1), le comptage est effectué lorsque le Tripode est activé par le client. Sur un CAB en entrée ou sortie contrôlée, le comptage est, théoriquement, identique aux nombre de validations. Sur un CAB positionné en sortie libre, il n’y a pas de données de validation mais il y a bien un comptage des franchissements.
	- Sur les CAB M1 nouvelle génération, un comptage des personnes qui franchissent l'obstable est réalisé, en plus des données de validation. Toute personne franchissant le passage est donc comptée, même si elle n’a pas validé. On compte donc tous les franchissements, en entrée/sortie, contrôlées comme libres.

- Les bornes qui ne bloquent pas le passage mais permettent de valider (c’est, en quelque sorte, un composteur pour Navigo). Elles permettent de remonter les validations télébilletiques.

Les données fournies dans un premier temps dans le cadre du Chalenge Digital SNCF concernent les données de validations et non de passages. Il est utile de préciser que de fortes lacunes peuvent exister dans ces données compte tenu de pannes, de maintenance, de fraude, etc.

Ces données permettent de connaître la technologie de validation (télébilletique ou magnétique), l’évènement associé (succès, échec, invalide, etc.), la zone du titre, le tarif associé, l’identifiant du valideur, le sens de passage, le vendeur du contrat, l’origine/destination du titre, l’identifiant de la carte/ticket etc. Notons que les identifiants clients sont modifiés tous les trois mois, pour des raisons de protection des données individuelles. Les données ne concernent que les validations SNCF. Elles sont disponibles sur la période janvier 2013-décembre 2014. 
