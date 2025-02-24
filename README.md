🚀 Comparaison des modèles ARIMA & Prophet pour optimiser les prévisions commerciales

📌 Contexte du projet
Dans un contexte commercial en constante évolution, il est crucial d'anticiper les ventes pour ajuster les stocks et les ressources. Ce projet vise à analyser et modéliser les tendances de vente en utilisant des modèles de séries temporelles et à comparer leurs performances.

🎯 Objectifs du projet
✔️ Analyser les tendances des ventes à partir de données historiques
✔️ Identifier les saisonnalités et les variations aléatoires
✔️ Construire et optimiser des modèles ARIMA et Prophet
✔️ Comparer la précision des prévisions et l'impact sur l'entreprise
✔️ Proposer des recommandations pour une meilleure prise de décision

📂 Données utilisées
📊 Dataset : Store Sales - Time Series Forecasting
Le jeu de données contient :

🏪 Ventes quotidiennes des magasins
📅 Date des transactions
🎉 Jours fériés et événements spéciaux
💰 Chiffres de vente par jour et par magasin
🔗 Source des données : Kaggle - Store Sales Forecasting

🔧 Technologies utilisées
✅ Python : Analyse et modélisation
✅ Pandas & NumPy : Manipulation des données
✅ Matplotlib & Seaborn : Visualisation des tendances
✅ Statsmodels : Modélisation ARIMA
✅ Facebook Prophet : Modélisation avancée avec Prophet
✅ Scikit-learn : Évaluation des modèles

🏗️ Architecture du projet
📂 dossiers et fichiers

bash
Copier
Modifier
📦 Prevision-des-Ventes
 ┣ 📂 data                        # Contient les données brutes et nettoyées
 ┣ 📂 notebooks                   # Contient les notebooks d'analyse et de modélisation
 ┣ 📂 visuals                     # Graphiques et visualisations générés
 ┣ 📜 requirements.txt            # Bibliothèques nécessaires
 ┣ 📜 README.md                   # Ce fichier
 ┣ 📜 arima_model.py              # Code de modélisation ARIMA
 ┣ 📜 prophet_model.py            # Code de modélisation Prophet
 ┣ 📜 evaluation.py               # Comparaison des modèles
 ┣ 📜 main.py                     # Script principal pour exécuter l'analyse
📈 Approche méthodologique
1️⃣ Exploration des données
Analyse des tendances, saisonnalité et bruit
Visualisation des séries temporelles
2️⃣ Test de stationnarité & transformation
Application du test ADF
Différenciation si nécessaire pour stationnariser les données
3️⃣ Modélisation avec ARIMA
Sélection automatique des hyperparamètres (p, d, q)
Ajustement et entraînement du modèle
4️⃣ Modélisation avec Prophet
Détection automatique de la tendance, saisonnalité, jours fériés
Entraînement et génération des prévisions
5️⃣ Comparaison des performances
📊 Métriques utilisées :
✔️ MAE (Mean Absolute Error)
✔️ RMSE (Root Mean Squared Error)
✔️ MAPE (Mean Absolute Percentage Error)

📌 Résultats et recommandations
✅ Prophet offre des prévisions plus précises avec un MAPE < 10%
✅ Il capture mieux la saisonnalité et les jours fériés qu'ARIMA
✅ Les erreurs (MAE, RMSE) sont plus faibles avec Prophet
⚠️ ARIMA reste plus performant pour les séries très stationnaires et les courtes prévisions

💡 Recommandation :
🔹 Utiliser Prophet pour des prévisions long terme et complexes
🔹 Envisager une hybridation avec ARIMA pour capturer les fluctuations soudaines

📎 Installation et utilisation
🔹 1. Cloner le dépôt
bash
Copier
Modifier
git clone https://github.com/ton-profil/Prevision-des-Ventes.git
cd Prevision-des-Ventes
🔹 2. Installer les dépendances
bash
Copier
Modifier
pip install -r requirements.txt
🔹 3. Exécuter le projet
Exécution complète
bash
Copier
Modifier
python main.py
Exécution des modèles individuels
bash
Copier
Modifier
python arima_model.py
python prophet_model.py
python evaluation.py
🔥 Contributions et améliorations
Toute contribution est la bienvenue ! 🛠️
📌 Idées d'amélioration :

Ajouter un modèle SARIMA pour comparer
Optimiser les hyperparamètres avec Grid Search
Intégrer un dashboard interactif avec Streamlit
📢 Contact & Partage
💡 Si ce projet t’a été utile, n’hésite pas à donner une étoile ⭐ sur GitHub !
