# Printer App — version publique

Application consacrée à la préparation et au pilotage de tâches d’impression.

## Confidentialité et anonymisation

Ce dépôt est une présentation publique de la structure du projet. **Tous les contenus d’origine des fichiers conservés ont été supprimés pour des raisons de confidentialité.** Les fichiers de code, de configuration, de migration SQL, de tests, de gouvernance et les artefacts d’ingénierie conservés contiennent uniquement la phrase « Contenu anonymisé ». Cette règle s’applique aussi aux exemples et aux modèles.

Les données, secrets, fichiers binaires, dépendances embarquées, résultats générés, wireframes, journaux et dossiers de documentation de work ont été exclus. Les dossiers `.agent` et `.agents`, les fichiers `AGENTS.md` et les métadonnées Git d’origine sont absents. Les noms susceptibles de révéler une entreprise, une personne, un client ou un système interne ont été remplacés par des noms génériques.

Seuls ce README et les présentations d’architecture ont un contenu explicatif : ces textes ont été entièrement rédigés pour cette version publique, sans reprendre les détails internes. L’historique Git public commence avec cette version anonymisée.

## Fonctionnement général

Deux ensembles présentent les rôles d’administration et d’utilisation. Les sous-dossiers exposent les couches applicatives, les interfaces, les services et les tests. Les formats d’impression et les traitements métier sont masqués.

Formats techniques représentés : Python, C# / .NET, C, XAML, scripts shell, configuration textuelle.

La copie permet de parcourir l’organisation technique et d’identifier les familles de composants. **Elle ne permet ni d’exécuter ni de reconstruire le projet.** Les configurations et les migrations sont volontairement incomplètes et ne doivent pas être lancées.

## Organisation

- `MakeFile`
- `administration/`
- `docs/`
- `operateur/`

Les noms `module-…` et `fichier-…` désignent des éléments renommés. Les extensions des fichiers textuels conservés indiquent leur format d’origine.

Consulter [ARCHITECTURE.md](ARCHITECTURE.md) pour la présentation générale.
