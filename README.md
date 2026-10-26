# PieceOut - Jeu de puzzle en C++

**PieceOut** est un projet universitaire de programmation orientée objet réalisé à l'**Université Paris Cité**. Inspiré des pièces de Tetris, ce jeu de réflexion propose **quatre puzzles** dans lesquels le joueur manipule des pièces pour atteindre une configuration cible.

Le projet a été développé en binôme par **Fatoumata Ndour** et **Abdoulbasti Mukaila Alh Shittu**.

## 🎮 Démonstration du jeu
[Capture vidéo du 2026-10-26 11-59-40.webm](https://github.com/user-attachments/assets/383fede2-07b8-4273-b683-84c0f47a8704)

## Fonctionnalités

- Interface graphique interactive développée avec **SFML**.
- Quatre puzzles accessibles depuis l'interface du jeu.
- Manipulation des pièces par **déplacement**, **rotation** et **symétrie**, selon les règles de chaque puzzle.
- Modélisation orientée objet des pièces, des opérations et du plateau.

## Technologies et concepts

- **Langage :** C++11
- **Interface graphique :** SFML (graphismes, fenêtres, audio)
- **Compilation :** GNU Make et g++
- **Programmation orientée objet :** classes, héritage, polymorphisme et gestion des objets
- **Patrons de conception abordés :** Decorator et Visitor

## Organisation du projet

```text
include/
  Modele/       # Déclarations des classes du modèle
  Vue/          # Déclarations des composants graphiques
source/
  Modele/       # Logique des pièces, opérations et plateau
  Vue/          # Interface graphique et quatre puzzles
ressources/     # Images et sons du jeu
Makefile        # Règles de compilation
Rapport PieceOut.pdf
Projet2024.pdf
```

Les fichiers `ebaucheModel.cpp` et `ebaucheVue.cpp` correspondent aux ébauches fournies dans le cadre du projet pédagogique.

## Prérequis

Un compilateur **g++** compatible C++11, **GNU Make** et les bibliothèques de développement **SFML** sont nécessaires. Les commandes ci-dessous correspondent à la configuration prévue dans le Makefile du projet ; la compilation n'a pas encore été revérifiée sur un environnement neuf.

## Compiler et lancer le jeu

À la racine du dépôt :

```bash
make all_vue
```

Le Makefile compile le jeu puis tente de lancer l'exécutable. Pour le relancer ensuite :

```bash
./build/ProgramVue
```

Pour nettoyer les fichiers générés :

```bash
make clean_modele
make clean_vue
```

> **Remarque :** les ressources graphiques et sonores doivent rester accessibles aux chemins attendus par le programme. Le fonctionnement dépend également de la version de SFML installée.

## Documentation

- **Rapport PieceOut.pdf** : rapport de réalisation du projet.
- **Projet2024.pdf** : sujet pédagogique initial.
- **architecturePieceOut-diagramme modele.drawio.jpg** : diagramme d'architecture du modèle.
- **README.pdf** : documentation complémentaire fournie avec le projet.

<details>
<summary><strong>Solutions détaillées des quatre puzzles</strong></summary>

Les étapes suivantes sont reprises de la documentation originale du projet.

### Puzzle 1
1. Une rotation sur la pièce verte.
2. Une rotation suivie d'un déplacement vers le haut sur la pièce bleue.
3. Une rotation sur la pièce verte.
4. Trois déplacements vers la gauche de la pièce jaune.
5. Une rotation de la pièce verte.
6. Enfin, six déplacements vers le haut de la pièce rouge.

### Puzzle 2
1. Une rotation suivie d'un déplacement à gauche de la pièce rouge.
2. Un déplacement en haut suivi d'une symétrie horizontale de la pièce verte.
3. Deux rotations successives de la pièce violette.
4. Une symétrie horizontale suivie de trois déplacements, puis une autre symétrie horizontale de la pièce verte.
5. Un déplacement vers la droite suivi d'une rotation, puis cinq déplacements vers le bas de la pièce rouge.

### Puzzle 3
1. Une symétrie verticale de la pièce violette.
2. Trois déplacements vers le haut de la pièce bleue.
3. Un déplacement vers le bas de la pièce jaune.
4. Deux rotations de la pièce bleue.
5. Deux déplacements vers la droite de la pièce rouge.
6. Deux déplacements vers le bas de la pièce violette.
7. Une rotation suivie de trois déplacements vers la gauche, puis une rotation de la pièce bleue.
8. Deux déplacement vers le haut de la pièce violette.
9. Trois déplacements vers le haut, suivis d'un déplacement vers la droite, puis un déplacement en haut de la pièce rouge.
10. Trois déplacements vers le bas, suivis d'une symétrie de la pièce violette.
11. Deux rotations suivies de deux déplacements vers le bas de la pièce bleue.
12. Enfin, quatre déplacements vers la gauche de la pièce rouge.

### Puzzle 4
1. Deux déplacements vers le bas suivis de deux rotations de la pièce verte.
2. Quatre déplacements vers le bas, suivis d'une rotation et d'un déplacement vers la droite de la pièce bleue.
3. Une rotation suivie d'un déplacement vers la gauche, une rotation, puis deux déplacements vers le haut de la pièce verte.
4. Deux déplacements vers le bas, suivis d'une rotation et de trois déplacements vers la droite de la pièce rouge.
5. Une rotation de la pièce bleue.
6. Une rotation suivie de deux déplacements de la pièce rouge.
7. Une rotation suivie d'un déplacement à gauche, une rotation, deux déplacements en bas, une rotation, un déplacement à gauche, trois rotations, puis deux déplacements vers le bas de la pièce verte.


</details>

## Auteurs

- **Fatoumata Ndour**
- **Abdoulbasti Mukaila Alh Shittu**

*Projet universitaire - Université Paris Cité.*
