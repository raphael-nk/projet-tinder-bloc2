## **Projet Tinder - Bloc 2 (EDA & Storytelling)**

![Logo Tinder](outputs/images/logo-tinder.png)

### **A propos de Tinder**

Tinder est une application de rencontre et de reseau social geolocalise.  
Les utilisateurs peuvent:
- **swiper a droite** pour indiquer un interet,
- **swiper a gauche** pour indiquer un refus,
- consulter des profils composes de photos, d'une courte bio et d'interets.

---

### **Objectif du projet**

Utiliser le dataset de speed dating pour comprendre ce qui favorise l'interet mutuel entre deux personnes et augmente la probabilite d'accepter un second rendez-vous.

---

### **Livrables attendus**

Un notebook contenant:
- des **statistiques descriptives**,
- des **visualisations**,
- des **legendes et interpretations** expliquant en quoi les indicateurs et les graphes eclairent l'acceptation d'un second rendez-vous.

Dans ce projet, les livrables principaux sont:
- `notebooks/03_full_eda.ipynb` : analyse exploratoire complete,
- `notebooks/04_data_storytelling.ipynb` : narration structuree orientee prise de decision.

---

### **Perimetre fonctionnel**

- Charger et exploiter un jeu de donnees nettoye de speed dating.
- Etudier les facteurs associes a `match` (interet mutuel).
- Produire des visualisations lisibles et interpretees.
- Structurer un fil narratif clair pour la restitution.
- Exporter les visuels utiles dans `outputs/images` avec un nommage explicite (`viz_*`).

Hors perimetre:
- modelisation predictive avancee,
- deploiement applicatif,
- collecte de nouvelles donnees.

---

### **Stack technique**

- **Python 3.12**
- **Pandas** (manipulation et analyse de donnees)
- **Plotly** (visualisations interactives)
- **Kaleido** (export d'images Plotly)
- **Jupyter Notebook / JupyterLab** (execution des notebooks)
- **uv** (gestion de l'environnement et des dependances)

---

### **Prerequis et installation**

#### **1. Prerequis**

- Python `3.12+`
- `uv` installe sur la machine

#### **2. Installation**

Depuis la racine du projet:

```bash
uv sync
```

---

### **Configuration et lancement**

Ouvrir et lancer les notebooks dans cet ordre conseille:
1. `notebooks/01_data_exploration.ipynb`
2. `notebooks/02_data_cleaning_norm.ipynb`
3. `notebooks/03_full_eda.ipynb`
4. `notebooks/04_data_storytelling.ipynb`
---

### **Structure du projet**

```text
notebooks/
  01_data_exploration.ipynb
  02_data_cleaning_norm.ipynb
  03_full_eda.ipynb
  04_data_storytelling.ipynb

outputs/
  data/
    df_speed_dating_prep.csv
    df_speed_dating_cleaned.csv
  images/
    logo-tinder.png
    viz_*.png
```

---

### **Points importants**

- La source principale analysee est `outputs/data/df_speed_dating_cleaned.csv`.
- Les exports de la partie storytelling suivent la convention `viz_<theme>_<message>.png`.
- Si un export Plotly echoue avec Kaleido, verifier l'installation de Kaleido/Chromium selon l'environnement.

---

### Auteur / Contexte

Projet realise dans le cadre de la certification CDSD (Jedha), Bloc 2: Exploratory Data Analysis.
