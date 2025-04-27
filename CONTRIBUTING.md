# Guide de contribution à MusicMind Player

Merci de votre intérêt pour contribuer à MusicMind Player ! Ce document fournit les directives pour participer au développement de cette application de lecteur de musique intelligent.

## 🌱 Démarrage

### Prérequis
- Node.js (version 18 ou supérieure)
- npm ou yarn
- Git
- Connaissance de base de React et Electron (pour le frontend)
- Connaissances en JavaScript/TypeScript

### Installation
1. Fork ce dépôt
2. Clonez votre fork localement
   ```bash
   git clone https://github.com/votre-username/music_player_idea.git
   cd music_player_idea
   ```
3. Installez les dépendances
   ```bash
   npm install
   # ou
   yarn install
   ```

## 🔍 Structure du projet

```
music_player_idea/
├── src/                      # Code source
│   ├── main/                 # Processus principal Electron
│   ├── renderer/             # Interface utilisateur React
│   ├── core/                 # Logique métier principale
│   │   ├── player/           # Moteur de lecture audio
│   │   ├── library/          # Gestion de la bibliothèque
│   │   └── smart-playlists/  # Système de playlists intelligentes
│   └── data/                 # Gestion des données et stockage
├── assets/                   # Ressources statiques
├── docs/                     # Documentation supplémentaire
├── tests/                    # Tests unitaires et d'intégration
├── scripts/                  # Scripts utilitaires
└── plugins/                  # Extensions et plugins
```

## 🚀 Cycle de développement

### Branches
- `main` - Branche principale, toujours stable
- `develop` - Branche de développement
- `feature/xxx` - Pour les nouvelles fonctionnalités
- `bugfix/xxx` - Pour les corrections de bugs
- `docs/xxx` - Pour les mises à jour de documentation

### Workflow de contribution
1. Créez une issue décrivant le problème ou la fonctionnalité
2. Créez une branche à partir de `develop`
3. Développez et testez votre contribution
4. Soumettez une Pull Request vers `develop`
5. Attendez la revue et l'approbation

### Conventions de codage
- **JavaScript/TypeScript** : Suivre les règles ESLint du projet
- **CSS/SCSS** : Utiliser l'approche BEM (Block Element Modifier)
- **React** : Privilégier les composants fonctionnels et hooks
- **Tests** : Chaque nouvelle fonctionnalité doit être accompagnée de tests

## 🎯 Domaines de contribution

### Interface utilisateur
- Amélioration du design et de l'expérience utilisateur
- Optimisation des performances d'interface
- Ajout de nouveaux thèmes et personnalisations

### Moteur de lecture
- Support de nouveaux formats audio
- Optimisation de la lecture et du décodage
- Ajout de fonctionnalités comme l'égaliseur ou les effets

### Gestion de bibliothèque
- Amélioration des algorithmes d'indexation
- Ajout de fonctionnalités de métadonnées
- Optimisation des performances de recherche

### Système de playlists intelligentes
- Nouveaux algorithmes de recommandation
- Amélioration des analyses musicales
- Nouvelles règles et contraintes pour les playlists

### Documentation et tests
- Amélioration de la documentation
- Expansion des tests unitaires et d'intégration
- Tutoriels et exemples d'utilisation

## 📝 Standards des Pull Requests

### Titre
Un titre clair qui décrit brièvement les changements, ex: "Ajouter le support FLAC" ou "Corriger le crash lors de l'importation de playlists"

### Description
- **Problème** : Décrivez le problème que vous résolvez
- **Solution** : Expliquez votre approche
- **Tests** : Comment avez-vous testé ces changements ?
- **Screenshots** : Si pertinent pour les changements d'interface
- **Issue** : Référence à l'issue concernée (#xx)

## 🧪 Tests

Nous utilisons Jest pour les tests unitaires et Cypress pour les tests d'interface. Exécutez les tests avant de soumettre une PR:

```bash
npm run test
# ou
yarn test
```

## 📚 Documentation

La documentation est essentielle. Si vous ajoutez une nouvelle fonctionnalité, assurez-vous de:
- Mettre à jour les fichiers README pertinents
- Documenter les fonctions et méthodes importantes
- Ajouter des commentaires pour le code complexe
- Mettre à jour la documentation des API si nécessaire

## 🔒 Sécurité

Si vous découvrez une vulnérabilité de sécurité, n'ouvrez PAS d'issue publique. Envoyez plutôt un email à [security@musicmind.example.com](mailto:security@musicmind.example.com).

## 📜 Licence

En contribuant à ce projet, vous acceptez que vos contributions soient licenciées sous la même licence que le projet (MIT).

## 🙏 Remerciements

Un grand merci à tous les contributeurs qui aident à faire de MusicMind Player une réalité !

---

N'hésitez pas à suggérer des améliorations à ce guide de contribution en ouvrant une issue ou une PR.
