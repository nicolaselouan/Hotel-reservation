Le projet serait de travailler ces valeurs SHAP en profondeur afin de répondre à la problématique : Les comportements de réservation sont-ils plus impactants que d'autres paramètres sur le maintien d'une réservation d'un hôtel ?
 
Pour répondre à cette problématique, les grandes étapes de la démarche sont ainsi : 
- Création d'un modèle de classification binaire performant.
- Regroupement de mes variables prédictives en type de variables (par exemple variables socio-démographiques, variables de type d'hôtels, variables de caractéristique du séjour... et variables de comportements de réservation).
- Evaluation des Mean Absolute SHAP Values de ces types de variables.
- Etude statistique sur les SHAP Values pour déterminer si les différences de Mean Absolute SHAP Values éventuellement constatées sont en effet significatives (test de Student -> test de Shapiro Wilk ou Q-Q plot + test de Levene).
 
Si les Mean Absolute SHAP Values placent les variables de comportement de réservation en première position et que les tests statistiques démontrent que la différence observée avec le deuxième groupe de variables est significative, alors la problématique sera validée.

Lien du dataset : https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand/data
