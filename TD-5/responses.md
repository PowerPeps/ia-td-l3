 Exercice 1 : Insuffisance rénale
 Taille du dataset et valeurs manquantes

Le dataset contient un certain nombre de patients décrits par plusieurs variables médicales.
On observe la présence de valeurs manquantes dans certaines colonnes, ce qui peut impacter les performances des méthodes d’apprentissage.

Importance des variables

Les valeurs maximales des variables montrent des différences d’échelle importantes entre les features.
Certaines variables, comme le nombre de globules blancs, ont des valeurs beaucoup plus élevées que d’autres.
Cela peut fortement influencer les distances utilisées en clustering et biaiser les résultats.

 Dendrogramme

Le dendrogramme met en évidence plusieurs regroupements possibles.
Une coupure de l’arbre permet d’obtenir environ 3 clusters, ce qui correspond au choix effectué pour la suite de l’analyse.

 Clustering (3 classes)

Un clustering hiérarchique a été réalisé avec 3 clusters à l’aide de la méthode AgglomerativeClustering.

 Analyse des clusters

D'apres mes resulatas obtenue je remarque : 

Le cluster 1 regroupe uniquement des patients atteints d’insuffisance rénale, ce qui montre une bonne séparation pour ce groupe.

Le cluster 0 contient majoritairement des patients malades mais également des patients sains, ce qui indique une séparation imparfaite.

Le cluster 2 présente une répartition presque équilibrée entre patients malades et non malades, ce qui montre qu’il est peu discriminant.

Globalement, la classification n’est pas totalement efficace, probablement à cause des différences d’échelle entre variables.
