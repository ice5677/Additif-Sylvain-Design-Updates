# latest.json

Le fichier `latest.json` est le manifeste lu par l’updater Tauri d’Additif Sylvain Design.

L’application est configurée pour consulter :

`https://github.com/ice5677/Additif-Sylvain-Design-Updates/releases/latest/download/latest.json`

Le manifeste publié doit décrire la version, les notes, la date de publication et la plateforme Windows x64, avec :

- l’URL HTTPS exacte de l’artefact de mise à jour publié dans la Release ;
- la signature Tauri correspondant exactement à cet artefact.

## Règle de version

Ne jamais publier comme « latest » une version égale ou inférieure à la version installée utilisée pour le test. Pour tester l’updater depuis ASD 0.3.2, la Release de test doit donc avoir une version supérieure.

## Validation

Avant publication, vérifier ensemble le nom réel de l’artefact généré et le contenu réel du fichier `.sig`. Ne jamais inventer une URL ou une signature.
