# **Распознавание автомобиля по его силуэту**
<a target="_blank" href="https://colab.research.google.com/github/VsevolodMus/Machine_Learning/blob/main/%D0%A0%D0%B0%D1%81%D0%BF%D0%BE%D0%B7%D0%BD%D0%B0%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5%20%D0%B0%D0%B2%D1%82%D0%BE%D0%BC%D0%BE%D0%B1%D0%B8%D0%BB%D1%8F/Vehicle.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>

### Метаданные

|Имя колонки|
|---|
COMPACTNESS
CIRCULARITY
DISTANCE_CIRCULARITY
RADIUS_RATIO
PR.AXIS_ASPECT_RATIO
MAX.LENGTH_ASPECT_RATIO
SCATTER_RATIO
ELONGATEDNESS
PR.AXIS_RECTANGULARITY
MAX.LENGTH_RECTANGULARITY
SCALED_VARIANCE_MAJOR
SCALED_VARIANCE_MINOR
SCALED_RADIUS_OF_GYRATION
SKEWNESS_ABOUT_MAJOR
SKEWNESS_ABOUT_MINOR
KURTOSIS_ABOUT_MAJOR
KURTOSIS_ABOUT_MINOR
HOLLOWS_RATIO
Class

**846 строк** - Каждая строка представляет собой один силуэт автомобиля.

**19 столбцов**

### Цель проекта

Определить класс автомобиля по набору данных, описывающих геометрические особенности силуэтов автомобилей, полученных из фотографий с распознаванием изображений.

### Инструменты
- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `sklearn`
- `stats`

## Заключение
1. Применялась многоклассовая классификация.

2. В наборе данных классы были сбалансированы.
    
3. Для процесса ML использовалась модель SVC.

4. Результаты:
    * Train/Test split: test_size=0.24, random_state=0;
    * SVC linear model показывает достаточно хорошую метрику accuracy = 80.8%;
    * Сonfusion matrix показывает, что из 204 примеров тестовых данных были верно определены 165 примеров и неверно определены 39 примеров;
    * Сonfusion matrix так же показывает, что самыми хорошо определяемыми классами являются "van" и "bus", а самыми трудно определяемыми "saab" и "opel".
