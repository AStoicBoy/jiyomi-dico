# Dictionnaires Jiyomi

Ce dépôt ne contient pas de code : il sert uniquement à distribuer les bases
de dictionnaire que l'application [Jiyomi](https://github.com/AStoicBoy/jiyomi)
télécharge à son premier lancement, une par langue.

Tout se trouve dans la **dernière release** :

- `manifest.json` — la liste des langues disponibles, ce que chaque base pèse
  et ce qu'elle couvre. C'est le seul fichier que l'app interroge.
- `jiyomi-dict-<langue>.db.gz` — la base elle-même, une par langue, au format
  SQLite compressé.

Ces fichiers sont fabriqués automatiquement et remplacés à chaque publication.
Les modifier à la main n'a pas de sens : ils repartiraient à la construction
suivante.

## Source et licence des données

Les données viennent de **JMdict**, publié par l'*Electronic Dictionary
Research and Development Group* sous licence
[Creative Commons Attribution-ShareAlike 4.0](https://creativecommons.org/licenses/by-sa/4.0/).

Source : <https://www.edrdg.org/jmdict/j_jmdict.html>

Les bases publiées ici en sont une œuvre dérivée : elles sont distribuées sous
la **même licence CC BY-SA 4.0**. Les sens ajoutés par traduction automatique
sont marqués comme tels dans la base, et signalés à l'utilisateur dans l'app.
