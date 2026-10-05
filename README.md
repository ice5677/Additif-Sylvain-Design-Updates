# Additif Sylvain Design — Canal de mises à jour

Dépôt public réservé à la distribution des mises à jour signées de **Additif Sylvain Design**.

## Principe

- Le code source reste dans le dépôt privé ASD.
- Ce dépôt public ne contient aucune donnée client.
- Les versions Windows sont publiées sous forme de **GitHub Releases**.
- Chaque Release destinée à l’updater contient l’installateur signé, sa signature Tauri et `latest.json`.
- ASD consulte uniquement le canal de Release public pour rechercher une version plus récente.

## Flux de publication

1. Compiler et signer ASD dans le dépôt privé.
2. Vérifier l’installateur Windows.
3. Créer une Release `vX.Y.Z` dans ce dépôt.
4. Joindre l’installateur signé et sa signature.
5. Générer et joindre `latest.json`.
6. Publier la Release.
7. Tester depuis la version ASD précédente : recherche, sauvegarde, installation, redémarrage et conservation des données.

## Sécurité

La clé privée de signature Tauri et son mot de passe ne doivent jamais être ajoutés à ce dépôt. Seule la clé publique est embarquée dans l’application.

Voir `docs/RELEASE-CHECKLIST.md` et `docs/LATEST-JSON.md` pour la procédure.
