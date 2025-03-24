# SemVer 📦🔢

**Le versionnage sémantique** (ou **SemVer**, pour _Semantic Versioning_) est un système standardisé pour attribuer des numéros de version aux logiciels, facilitant la compréhension des modifications apportées entre chaque version.

## Structure d'une version SemVer

Une version SemVer se compose de trois nombres séparés par des points : **MAJEUR.MINEUR.CORRECTIF** (par exemple, `1.4.2`). Chaque segment indique le type de changement effectué :

1. **MAJEUR** (_MAJOR_) : Incrémenté lors de modifications incompatibles avec les versions précédentes.

2. **MINEUR** (_MINOR_) : Incrémenté lors de l'ajout de nouvelles fonctionnalités compatibles avec les versions antérieures.

3. **CORRECTIF** (_PATCH_) : Incrémenté lors de corrections de bugs ou d'améliorations mineures, tout en maintenant la compatibilité existante.

Par exemple, la version `2.3.1` correspond à la deuxième version majeure, avec trois ajouts mineurs et un correctif.

## Versions préliminaires et métadonnées

SemVer permet également d'ajouter des identifiants pour préciser l'état d'une version :

-   **Versions préliminaires** : Ajoutées après un tiret, elles indiquent des versions non stables destinées aux tests (par exemple, `1.0.0-alpha.1`).

-   **Métadonnées de build** : Ajoutées après un signe plus, elles fournissent des informations supplémentaires sur la build (par exemple, `1.0.0+20130313144700`).

## Avantages du versionnage sémantique

-   **Clarté** : Les numéros de version reflètent clairement la nature des modifications, aidant les développeurs et les utilisateurs à comprendre les évolutions du logiciel.

-   **Gestion efficace des dépendances** : Les systèmes de gestion de paquets peuvent déterminer automatiquement les mises à jour compatibles, réduisant les risques de conflits.

-   **Communication améliorée** : Une convention standardisée aligne les attentes entre les équipes de développement et les utilisateurs concernant les mises à jour logicielles.

## Conclusion

Adopter le versionnage sémantique offre une structure claire et prévisible pour la gestion des versions logicielles, facilitant la maintenance et l'évolution des projets.

Pour approfondir, vous pouvez consulter la spécification officielle : [semver.org](https://semver.org/lang/fr/)
