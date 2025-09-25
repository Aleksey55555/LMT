# Logistic Model Tree (LMT): Experiments

## 📌 Описание
Этот репозиторий содержит экспериментальное исследование **Logistic Model Tree (LMT)** — гибридной модели, которая объединяет:
- структуру дерева решений (деление по признакам);
- логистическую регрессию в листьях (для локального обучения).

Реализация LMT выполненас использованием `scikit-learn` API, также приведено её сравнение с классическими моделями:  
- Logistic Regression  
- Random Forest  
- XGBoost  

В экспериментах рассматривались:
- Бинарная классификация: **Breast Cancer** (из sklearn.datasets)  
- Мультиклассовая классификация: **Wine** (из sklearn.datasets)  
- Синтетический датасет (`make_classification`)  

Также протестированы ансамбли:
- **LMT-Bagging** (через `BaggingClassifier`)  
- **LMT-Boosting**
- **Gradient Boosting (LogitBoost-style) с LMT-листами**
