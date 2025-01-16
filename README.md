# YourAgenda
Un site pour developper de nouvelles compétences

## Prompt pour Générer un Planning d'Apprentissage JSON sur chatgpt

Utilisez ce prompt pour générer automatiquement un planning structuré d'apprentissage sous forme de fichier JSON nommé **`planning.json`**. Le planning inclut des journées d'apprentissage, de révision, de repos, ainsi qu'une section dédiée aux ressources.

---

### **Prompt :**

Je souhaite apprendre **[sujet]** et je dispose de **[durée]** par jour pour cela. Mon objectif est de structurer mon apprentissage de manière claire, organisée et efficace, en couvrant à la fois la théorie, la pratique et les révisions.  
Génère un planning complet sous forme de JSON, avec la **structure suivante**, et enregistre-le automatiquement dans un fichier nommé **`planning.json`** :  

- **`daily_schedule`** :
  - **`learning_days`** :
    - Inclure une clé `total_duration` correspondant à la durée totale d'apprentissage par jour.
    - Une liste de `sessions`, où chaque session est définie par :
      - `duration` : Durée de la session.
      - `activity` : Activité principale.
      - `details` : Liste des sous-activités ou thèmes abordés.
  - **`revision_day`** :
    - Inclure une clé `total_duration` correspondant au temps total des révisions.
    - Une liste de `sessions` définissant les activités spécifiques de révision avec :
      - `duration` : Durée de la session.
      - `activity` : Nom de l’activité.
  - **`rest_day`** :
    - Inclure une liste d’activités optionnelles définies par :
      - `duration` : Durée de l’activité.
      - `activity` : Description de l’activité.
    - Ajouter une note de repos expliquant l’importance de recharger les batteries.

- **`resources`** : Une section rassemblant des recommandations utiles pour ce sujet, comprenant :
  - **`online_courses`** : Une liste de cours en ligne avec les champs :
    - `name` : Nom du cours.
    - `platform` : Plateforme où le cours est disponible.
    - `link` : Lien direct vers le cours.
  - **`books`** : Une liste de livres utiles avec les champs :
    - `title` : Titre du livre.
    - `author` : Auteur du livre.
    - `description` : Courte description ou intérêt pour le sujet.
  - **`practice_platforms`** : Une liste de plateformes pour la pratique avec les champs :
    - `name` : Nom de la plateforme.
    - `description` : Ce qu’elle propose.
    - `link` : Lien vers la plateforme.

Adapte le contenu du JSON à mon sujet et à la durée spécifiée, tout en garantissant que la structure reste identique. Enregistre automatiquement ce JSON dans un fichier nommé **`planning.json`**.

---

### **Exemple d’utilisation :**

- Sujet : **Design UX/UI**
- Durée : **3 heures**

Le JSON généré sera structuré comme suit :
- Une clé `daily_schedule` contenant :
  - Des journées d'apprentissage (learning_days).
  - Un jour de révision (revision_day).
  - Un jour de repos (rest_day).
- Une clé `resources` listant les cours en ligne, livres, et plateformes pertinentes.

---

Copiez ce prompt, personnalisez-le avec votre sujet et votre durée, et laissez l'outil générer automatiquement votre fichier `planning.json` ! 🚀
