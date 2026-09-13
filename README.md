# 🛡️ Détection d'intrusions dans un réseau (IDS) — Deep Learning & ML

Détection de **comportements malveillants** dans le trafic réseau, en binaire (normal / anormal) et **multi-classes** (DoS, Probe, U2R, R2L), via **Machine Learning et réseaux de neurones**.

---

## 🇫🇷 Français

### 🎯 Objectif
Identifier automatiquement les **attaques réseau** et leur type, à partir de données de trafic (style NSL-KDD), avec une forte exigence de **précision** tout en documentant les classes rares difficiles.

### 🏗️ Démarche
1. **Analyse des données** — étude univariée, distribution des classes (normal + 4 types d'attaques).
2. **Prétraitement** — binning de la durée (`duration_bin`), encodage des protocoles/services.
3. **Modélisation** — **KNN** (binaire + multi-classes) puis **réseaux de neurones MLP/CNN** (TensorFlow/Keras).
4. **Évaluation** — précision, rappel, F1-score, rapports de classification par classe.

### 🛠️ Technologies
Python · scikit-learn (KNN, métriques) · TensorFlow / Keras · pandas · matplotlib / seaborn

### 📊 Résultats
| Approche | Précision binaire | Précision multi-classes |
|---|---|---|
| **KNN** (scikit-learn) | **≈ 99,60 %** | **≈ 99,57 %** |
| **Réseau de neurones** (MLP/CNN) | **≈ 97,4 %** | **≈ 99,25 %** |

- F1 pondéré ≈ 0,98–0,99 ; les classes **rares** (U2R, R2L) restent sous-performantes — limite analysée et documentée.

---

## 🇬🇧 English

### 🎯 Objective
Automatically detect **network attacks** and their type from traffic data (NSL-KDD-style), in binary (normal / abnormal) and **multi-class** settings (DoS, Probe, U2R, R2L), with a strong focus on **precision** while documenting hard rare classes.

### 🏗️ Approach
1. **Data analysis** — univariate exploration, class distribution (normal + 4 attack types).
2. **Preprocessing** — duration binning (`duration_bin`), protocol/service encoding.
3. **Modelling** — **KNN** (binary + multi-class) then **MLP/CNN neural networks** (TensorFlow/Keras).
4. **Evaluation** — precision, recall, F1-score, per-class classification reports.

### 🛠️ Tech Stack
Python · scikit-learn (KNN, metrics) · TensorFlow / Keras · pandas · matplotlib / seaborn

### 📊 Results
| Approach | Binary accuracy | Multi-class accuracy |
|---|---|---|
| **KNN** (scikit-learn) | **≈ 99.60%** | **≈ 99.57%** |
| **Neural network** (MLP/CNN) | **≈ 97.4%** | **≈ 99.25%** |

- Weighted F1 ≈ 0.98–0.99; **rare classes** (U2R, R2L) remain underperforming — a limitation analysed and documented.

---

### 🗂️ Notes
6 notebooks exploratoires (`Intrusion*.ipynb`, `IntrusionBin`, `IntrusionMul`) couvrant analyses, préparation et modèles. / 6 exploratory notebooks covering analysis, preparation and models.