# ali-ca

La liste des aliments est enregistrée dans le stockage local du navigateur et rechargée au démarrage. Le bouton « Sauvegarder les aliments » enregistre la liste actuelle ; les ajouts personnalisés sont aussi enregistrés automatiquement. Au premier lancement, `aliments.json` fournit la liste initiale et les anciens aliments personnalisés sont conservés. La page et ce fichier doivent être accessibles depuis le même site.

La sauvegarde reste propre au navigateur et à l'appareil : elle peut être effacée avec les données du site et n'est pas synchronisée automatiquement entre appareils.

Dans les sauvegardes JSON et CSV, la date et l'heure de chaque aliment sont au format `yymmdd-hhmmss`. Les anciennes entrées ne conservaient pas les secondes : elles sont exportées avec `00` pour les secondes.

Dans le CSV, la première colonne `date` utilise le format `dd.mm.yy`.