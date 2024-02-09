# Résolution last exercice:

Pour la fonction main:
Modification pour renvoyer Result<(), Box<dyn error::Error>> en indiquant qu'elle peut maintenant produire des erreurs.
Conversion de la chaîne de caractères pretend_user_input en un i64 est maintenant gérée avec l'opérateur ? afin que tout échec de conversion entraînera la propagation de l'erreur.

Le type d'erreur CreationError a été ajouté pour représenter les erreurs spécifiques à la création de l' i64, telles que les valeurs négatives ou nulles.
Une implémentation de Display et Error a été ajoutée à CreationError pour formater et afficher les messages d'erreur de manière plus conviviale.

Pour la fonction parse_pos_nonzero :
    La fonction renvoie maintenant un Result avec le type d'erreur ParsePosNonzeroError.
    La conversion de la chaîne de caractères i64 est désormais gérée avec s.parse()?, et en cas d'échec, une erreur ParsePosNonzeroError::ParseInt est retournée.
