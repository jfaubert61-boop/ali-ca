# ali-ca

La liste des aliments est enregistrée dans le stockage local du navigateur et rechargée au démarrage. Le bouton « Sauvegarder les aliments » enregistre la liste actuelle ; les ajouts personnalisés sont aussi enregistrés automatiquement. Au premier lancement, `aliments.json` fournit la liste initiale et les anciens aliments personnalisés sont conservés. La page et ce fichier doivent être accessibles depuis le même site.

La sauvegarde reste propre au navigateur et à l'appareil : elle peut être effacée avec les données du site et n'est pas synchronisée automatiquement entre appareils.

Pour modifier la liste dans OneDrive, cliquez sur « Télécharger listeAli.json », puis placez le fichier téléchargé dans `OneDrive/Import_1d` et modifiez-le avec un éditeur de texte. Après modification, cliquez sur « Charger listeAli.json » et sélectionnez ce fichier dans OneDrive. Après confirmation, sa liste remplace toute la liste de Safari, y compris les aliments personnalisés absents du fichier ; elle est sauvegardée localement et rechargée aux prochains démarrages. Le navigateur ne peut pas accéder automatiquement au dossier OneDrive.

Le fichier est un tableau JSON. Chaque aliment doit avoir un `id` unique (nombre ou texte), un `nom`, une `categorie` et un nombre `calories_100g` positif ou nul. Les champs numériques `portion_defaut`, `glucide`, `lipide` et `proteine` sont facultatifs et positifs ou nuls ; `unite` est facultatif. Le fichier téléchargé donne un exemple complet.

Dans les sauvegardes JSON et CSV, la date et l'heure de chaque aliment sont au format `yymmdd-hhmmss`. Les anciennes entrées ne conservaient pas les secondes : elles sont exportées avec `00` pour les secondes.

Dans le CSV, la première colonne `date` utilise le format `dd.mm.yy`.