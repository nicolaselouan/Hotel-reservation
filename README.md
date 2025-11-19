Le dataset sur lequel nous travaillons est issu d'une publication de Nuno Antonio, Ana Almeida et Luis Nunes pour Data in Brief (Volume 22, Février 2019). Ce dataset agrège les données résultantes de deux sources : la première d'un hôtel de campagne et la seconde d'un hôtel situé en ville.<br>
Le lien du dataset est le suivant : https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand/data

L'annulation d'une réservation séjour touristique peut-être multifactorielle : aléas familiaux, météorologiques, politiques... <br>
Cependant, d'aucuns pourraient penser qu'il est possible, de par certaines caractéristiques des clients ou de la réservation, de prédire si oui ou non un client sera enclin à annuler une réservation. Le dataset que nous utilisons fait l'objet de nombreux travaux étudiant cette question. <br>Afin d'aller au-delà, nous avons décidé d'étudier les valeurs SHAP dans le but de répondre à la problématique suivante : **Les comportements de réservation sont-ils plus impactants que d'autres paramètres sur le maintien d'une réservation d'un hôtel ?** <br> En effet, notre premier postulat face aux variables de ce dataset est qu'un client déjà reconnu comme ayant ou non annulé une réservation dans le passé sera ou non plus enclin à annuler une prochaine réservation et qu'ainsi les variables rendant compte de ces faits ont une importance plus grande que les autres dans la classification finale du modèle. 

Notre projet se déclinera de la sorte :
- Création d'un modèle de classification binaire performant (FAIT)
- Regroupement des variables prédictives en type de variables (par exemple variables socio-démographiques, variables de type d'hôtels, variables de caractéristique du séjour... et évidemment variables de comportements de réservation) (FAIT)
- Evaluation des Mean Absolute SHAP Values de chacun de ces groupes de variables (FAIT)
- Etude statistique sur les SHAP Values pour déterminer si les différences de Mean Absolute SHAP Values éventuellement constatées sont en effet significatives (test de Student -> test de Shapiro Wilk ou Q-Q plot + test de Levene) (EN COURS)
