# Checklist de publication ASD

Cette checklist est à suivre pour chaque nouvelle version distribuée par l’updater.

- [ ] La version est supérieure à celle actuellement installée.
- [ ] La compilation Windows x64 est terminée.
- [ ] L’installateur Tauri a été signé.
- [ ] Le fichier de signature `.sig` correspond exactement à l’installateur publié.
- [ ] Les notes de version sont prêtes.
- [ ] Une Release GitHub `vX.Y.Z` est créée.
- [ ] L’installateur signé est joint à la Release.
- [ ] `latest.json` pointe vers l’URL de téléchargement de cette même Release.
- [ ] La signature contenue dans `latest.json` est celle du fichier `.sig`.
- [ ] `latest.json` est joint à la Release.
- [ ] La Release est publiée.
- [ ] Depuis ASD : « Rechercher une mise à jour » détecte la nouvelle version.
- [ ] La sauvegarde locale est créée avant installation.
- [ ] L’installation et le redémarrage réussissent.
- [ ] Les clients, devis, factures et réglages existants sont toujours présents.

Ne jamais publier la clé privée de signature, son mot de passe, une base `workspace.db` ou une sauvegarde client.
