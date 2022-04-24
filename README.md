# SpringBootControl
une API REST avec Spring Boot pour la gestion d’une bibliothèque.


Exigences métiers :
• L’application doit permettre de gérer l’entité livre (Création, modification et suppression)
• Un livre est défini par :
o ID unique et s’incrémente d’une manière automatique.
o Titre d’une taille qui ne dépasse pas 50 caractères.
o Maison d’édition
o Date de sortie
o Auteur
o Nombre de page
o ISBN
o Date de la dernière consultation
o Un attribut pour représenter si le livre est disponible ou non
• La valeur de ISBN doit être unique.
• L’utilisateur ne peut pas insérer des valeurs nulles.
• L’utilisateur ne doit pas avoir la possibilité pour modifier les attributs « Maison d’édition » et
« ISBN » (utiliser le paramètre updatable)
• Les livres doivent être triés par ordre croissant, lors de la sélection. (Utiliser @OrderBy)
• On suppose que la base de données contient une liste des livres, pour manipuler son contenu :
o L’utilisateur peut avoir la liste des livres en utilisant l’url : emsi_api/livres
o L’utilisateur peut avoir la liste un livre en utilisant l’url : emsi_api/livres/{id}
o Suivez la même logique pour l’opération de modification et suppression.
