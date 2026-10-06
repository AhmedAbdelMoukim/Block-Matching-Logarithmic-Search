# Logarithmic Search Block Matching for Motion Estimation

Ce dépôt contient une implémentation en **Python** de l'algorithme de **recherche logarithmique (Logarithmic Search / 2D Logarithmic Search)** pour le *Block Matching* (appariement de blocs) et l'estimation de mouvement entre images successives[cite: 6].

---

## 📌 Présentation du Projet

L'estimation de mouvement par appariement de blocs est une technique essentielle dans la compression vidéo (ex: MPEG, H.264) et le traitement d'images. 

Plutôt que d'effectuer une recherche exhaustive (Full Search) très gourmande en calculs, l'algorithme de **recherche logarithmique** réduit considérablement la complexité temporelle en divisant le rayon de recherche à chaque étape de manière logarithmique jusqu'à trouver le bloc le plus similaire (basé sur l'erreur quadratique moyenne / MSE)[cite: 6].

---

## 🛠️ Fonctionnalités

- **Recherche Logarithmique Optimisée :** Algorithme rapide de recherche de vecteurs de mouvement à rayon variable[cite: 6].
- **Calcul de Métrique (MSE) :** Comparaison de blocs basée sur l'erreur quadratique moyenne (`np.mean`)[cite: 6].
- **Visualisation Dynamique :** Affichage côte à côte des blocs originaux et de leurs correspondances identifiées avec des couleurs distinctes[cite: 6].
- **Traitements d'Images avec OpenCV :** Manipulation efficace des grilles de blocs et affichage des résultats avec Matplotlib[cite: 6].

---

## 📂 Structure du Dépôt

```text
.
├── Logarithmique Search.py    # Script principal de l'algorithme de recherche logarithmique
├── Data/                      # Dossier contenant la séquence d'images d'entrée
└── README.md                  # Documentation du projet
```

---

## 📋 Prérequis & Installation

### 1. Cloner le dépôt

```bash
git clone [https://github.com/votre-utilisateur/logarithmic-search-block-matching.git](https://github.com/votre-utilisateur/logarithmic-search-block-matching.git)
cd logarithmic-search-block-matching
```

### 2. Installer les dépendances

Le projet nécessite Python 3.x et les bibliothèques suivantes :

```bash
pip install opencv-python numpy matplotlib
```

---

## 🚀 Utilisation

1. Placez vos images successives dans le dossier `Data/` (ou adaptez le chemin dans le script)[cite: 6].
2. Lancez le script Python :

```bash
python "Logarithmique Search.py"
```

3. Le programme affichera deux figures :
   - **Image 1 :** Les blocs découpés sur l'image source[cite: 6].
   - **Image 2 :** L'image cible avec les cadres de blocs correspondants identifiés par l'algorithme[cite: 6].

---

## 📄 Licence

Ce projet est sous licence [MIT](LICENSE) - libre d'utilisation, de modification et de distribution.
