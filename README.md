# 💡 Проект: Бинарная классификация для предиктивного обслуживания оборудования

## Цель
Разработка ML-модели для прогнозирования отказов промышленного оборудования с выводом в интерактивном Streamlit-приложении.

## Данные
**Датасет:** [UCI AI4I 2020 Predictive Maintenance Dataset](https://archive.ics.uci.edu/dataset/601/predictive+maintenance+dataset)  
**Характеристики:**
- 10,000 записей
- Признаки: температура, крутящий момент, скорость вращения, износ и др.
- Целевая переменная: `Machine failure` (бинарная)

## Техническая реализация
**Модель:** Random Forest Classifier  
**Метрики:**
- Accuracy: 0.98
- ROC-AUC: 0.96
- Confusion Matrix
- Classification Report

**Предобработка:**
1. Удаление нефункциональных признаков (UDI, Product ID)
2. One-Hot Encoding для категориальных переменных
3. Стандартизация числовых признаков

## Интерфейс
Streamlit-приложение включает:
- Загрузку пользовательских данных
- Визуализацию метрик модели
- Интерактивный ввод параметров оборудования
- Вывод прогноза вероятности отказа

## Запуск проекта
```bash
1. Клонируйте репозиторий:
git clone https://github.com/1-1ii/predictive_maintenance_shilkina.git
cd .\predictive_maintenance_shilkina
2. Установите зависимости:
pip install -r requirements.txt
3. Запустите приложение:
streamlit run app.py
```

## Видео демонстрация
[Видео работы приложения](video/demo.mp4)
<video src="video/demo.mp4" controls width="100%" poster="img/preview.jpg"></video>
