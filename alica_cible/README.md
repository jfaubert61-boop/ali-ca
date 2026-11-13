# alica_cible

Dossier du projet parallèle à ali-ca.

Le bouton « Importer ali_cible.json » affiche un tableau de quatre colonnes :
Kcal, Glucides (g), Lipides (g) et Protéines (g). Le fichier doit contenir un objet avec les champs
`Kcal`, `Glu`, `Lip g`, `Prot p`, `Glu %`, `Lip %` et `Prot %` dans une liste
`cible` contenant une seule cible. Les pourcentages sont affichés sur la
troisième ligne, avec une cellule vide sous Kcal.

Le bouton « Importer un JSON d’aliments » accepte une liste d'aliments, un
objet contenant une liste `repas` ou une sauvegarde `repasParJour`. Il affiche
la somme des calories, glucides, lipides et protéines. Sur iPhone, les deux
boutons ouvrent le sélecteur de fichiers natif.
