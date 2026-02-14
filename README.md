# Physics-Informed Neural Networks (PINNs) : Modélisation de Circuit RC

Ce dépôt présente une implémentation de **PINNs** appliquée à l'électrocinétique. L'objectif est de prédire la décharge d'un condensateur en intégrant la **loi de Kirchhoff** directement dans la fonction de perte du réseau de neurones.

## 🚀 Points Forts du Projet
- **Contrainte Physique** : Utilisation de l'équation différentielle $RC \frac{dV}{dt} + V = 0$ comme régulateur.
- **Efficacité Data** : Le modèle converge avec seulement **2 points de mesure bruités**, là où un réseau standard échoue.
- **Performance** : Convergence vers la solution exacte **2x plus rapide** (en termes d'erreur de généralisation).

## 📊 Résultats
Le modèle PINN filtre naturellement le bruit des capteurs et assure une extrapolation physiquement cohérente, contrairement aux approches "Data-driven" classiques qui souffrent d'overfitting sur des données rares.

## 🛠️ Installation
```bash
pip install -r requirements.txt
💻 Utilisation
Le code principal se trouve dans le notebook PINN_Convergence_Accélérée_par_Physique.ipynb.