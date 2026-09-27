# Reponses aux  questions du tp 




- Pour identifier une agence sans ambiguïté, le couple (nom, ville) doit être défini comme unique car deux agences de nom dans des villes différentes (ex: Ecobank Sokodé et Ecobank Lomé) constituent deux lieux d'accueil distincts pour les stagiaires.

- Le champ email utilise EmailField afin de déléguer la validation du format directement au framework Django plutôt que de réinventer un validateur sur du texte brut.

- Le secteur d'activité est laissé en texte libre car figer une liste de choix aujourd'hui bloquerait la saisie de secteurs imprévus par le secrétariat, quitte à devoir nettoyer les données ou migrer vers une table dédiée dans trois mois.


- La dernière phrase du secrétariat fait référence à la méthode magique __str__ qui surcharge l'affichage textuel par défaut de l'objet dans l'administration Django.
