# ali-ca

Dans les sauvegardes JSON et CSV, la date et l'heure de chaque aliment sont au format `yymmdd-hhmmss`. Les anciennes entrées ne conservaient pas les secondes : elles sont exportées avec `00` pour les secondes.

Dans le CSV, la première colonne `date` utilise le format `dd.mm.yy`.