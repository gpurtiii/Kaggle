# Kaggle
Cardiovascular Disease

## Introducció

El projecte aborda una tasca de **classificació supervisada**, seleccionant models com:
- Regressió Logística (*Logistic Regression*)
- *Support Vector Machine (SVM)*
- *K-Nearest Neighbors (KNN)*
- *Random Forest*

S'utilitza una combinació de tècniques com la validació creuada i l'optimització d'hiperparàmetres amb *RandomizedSearchCV* per maximitzar el F1-Score, prioritzant un bon equilibri entre precisió i *recall*.

## Dependències

El projecte utilitza **Python** i les següents biblioteques:
- `pandas`
- `numpy`
- `scikit-learn`
- `matplotlib`

## Descripció del projecte

### 1. Conjunt de dades
El dataset conté informació mèdica com:
- Edat, alçada, pes
- Pressió arterial sistòlica i diastòlica
- Variables categòriques com colesterol i glucosa
- Activitats com fumar, consum d'alcohol i exercici físic
- Variable objectiu: Presència o absència de malaltia cardiovascular.

### 2. Pipeline d'entrenament
- **Mostra del dataset**: Es treballa amb una mostra representativa de 10.000 files per accelerar el procés.
- **Divisió del dataset**: Es divideixen les dades en conjunts d'entrenament i prova (70%-30%).
- **Selecció de models**: Es proven 4 models de classificació.
- **Cerca d'hiperparàmetres**: S'utilitza *RandomizedSearchCV* per optimitzar els hiperparàmetres de cada model.
- **Mètrica principal**: El F1-Score s'utilitza per comparar els models.

### 3. Comparació de resultats
S'avaluen els models en termes de F1-Score i es selecciona el millor model amb els hiperparàmetres òptims.
