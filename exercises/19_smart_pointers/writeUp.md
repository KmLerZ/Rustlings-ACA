# Résolution last exercice:

Pour la fonction reference_mutation :
- Vérifie Cow::Owned(vec) pour s'assurer que la mutation du Cow conduit à la possession effective d'un vecteur, et utilise assert_eq! pour comparer le contenu du vecteur après la mutation.

Pour la fonction reference_no_mutation :
- Vérifie Cow::Borrowed(vec) pour s'assurer que lorsque le Cow n'est pas muté, il continue à emprunter les données et utilise assert_eq! pour comparer le contenu du vecteur.

Pour la fonction owned_no_mutation :
- Vérifie Cow::Owned(vec) pour s'assurer que lorsqu'un Cow possède déjà les données et qu'il n'y a pas de mutation, il continue à posséder les données, et utilise assert_eq! pour comparer le contenu du vecteur.

Pour la fonction owned_mutation :
- Vérifie Cow::Owned(vec) pour s'assurer que lorsqu'un Cow possède déjà les données et qu'il y a une mutation, il continue à posséder les données mutées, et utilise assert_eq! pour comparer le contenu du vecteur après la mutation.