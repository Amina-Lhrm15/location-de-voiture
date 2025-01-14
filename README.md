# location-de-voiture
int main : boucle 1 :Le programme lit chaque ligne du fichier pour voir si l'utilisateur existe déjà ;strtok extrait le nom et le mot de passe de chaque ligne. Si un nom correspond à celui saisi, found passe à 1 si non demande a utilisateur de saisir son age Si l'utilisateur a moins de 18 ans, il est informé qu'il ne peut pas louer une voiture.
Sinon, le programme demande s'il est en période d'essai :
Si non, il ne peut pas louer.
Sinon, il est invité à définir un mot de passe, qui sera enregistré dans le fichier de mode lecture et ecriture  sous la forme nom_prenom;mot_de_passe. Si l'utilisateur est trouvé dans le fichier, il doit entrer son mot de passe Tant que le mot de passe ne correspond pas, le programme lui redemande encore une fois de le saisir .Une fois utilisateur saisi ces informations , l'utilisateur accède au menu principal :Les options permettent de gérer les voitures selon leur catégorie (économique, moyenne ou luxe).
Chaque catégorie a ses propres fonctions, telles que economi() pour ajouter une voiture ou afficherVoitures1() pour afficher les voitures économiques.Pour chaque opération (ajouter, afficher, supprimer, modifier), l'utilisateur doit choisir une catégorie  c est a dire un numero parmi ces numeros .     
La structure voiture représente les informations d'une voiture. hada .h ID : Identifiant unique de la voiture.
marque : Marque de la voiture par exemple Toyota
model : Année du modèle par exemple 2020
nbredeplace : Nombre de places disponibles dans la voiture.
prjour  c est a dire Prix de location par jour.
typca : Type de carrosserie (exemple : berline).
trans : Type de transmission ; s il est  automatique ou manuelle.
dispo : Disponibilité de la voiture .Ces déclarations représentent les prototypes des fonctions utilisées dans le programme principal.economi() : Ajouter une voiture de categorie  économique.
moyenne() : Ajouter une voiture de catégorie moyenne.
luxe() : Ajouter une voiture de categorie luxe.Ces fonctions affichent les voitures disponibles selon leur catégorie :
afficherVoitures1() : Affiche les voitures économiques.
afficherVoitures2() : Affiche les voitures de catégorie moyenne.
afficherVoitures3() : Affiche les voitures de luxe.                
Ces fonctions suppriment une voiture spécifique selon sa catégorie :
supprimer_voiture1() : Supprime une voiture économique.
supprimer_voiture2() : Supprime une voiture de catégorie moyenne.
supprimer_voiture3() : Supprime une voiture de luxe.            
Ces fonctions modifient les informations d'une voiture selon sa catégorie :
modifierVoiture1() : Modifie une voiture économique.
modifierVoiture2() : Modifie une voiture de catégorie moyenne.
modifierVoiture3() : Modifie une voiture de luxe.  
Ajouter une voiture :
Les fonctions economi, moyenne, et luxe permettent d'ajouter des voitures à différents fichiers CSV : "economi.CSV", "moyenne.CSV", et "luxe.CSV".
Elles demandent à l'utilisateur d'entrer des informations sur la voiture (marque, modèle, ID, nombre de places, prix par jour, etc.).
Elles vérifient si une voiture avec la même marque existe déjà dans le fichier. Si c'est le cas, elles affichent un message et ne permettent pas l'ajout. Sinon, elles ajoutent les données dans le fichier.                                                                      
Les fonctions afficherVoitures1, afficherVoitures2 et afficherVoitures3 permettent d'afficher les voitures présentes dans les fichiers "economi.CSV", "moyenne.CSV", et "luxe.CSV" afficher la voiture avec ces informations.                                     
Les fonctions supprimer_voiture1, supprimer_voiture2, et supprimer_voiture3 permettent de supprimer une voiture d'un fichier en fonction de son ID.
Elles ouvrent le fichier en lecture et créent un fichier temporaire où toutes les voitures, sauf celle à supprimer, sont copiées.
Après avoir terminé la lecture, elles suppriment l'ancien fichier et renommer le fichier temporaire pour qu'il remplace l'ancien fichier.                                    
Les fonctions modifierVoiture1, modifierVoiture2, et modifierVoiture3 permettent de modifier les informations d'une voiture dans les fichiers respectifs.
Elles cherchent la voiture avec l'ID donné, et si trouvée, l'utilisateur peut modifier ses informations. Ensuite, les informations mises à jour sont écrites dans un fichier temporaire et l'ancien fichier est remplacé.                                           
Utilisation de fread et fwrite : Ces fonctions sont utilisées pour lire et écrire des structures de données de type voitur, qui représentent les informations d'une voiture. hada dak car.c
