# Детектирование кораблей, машин и самолётов на изображениях

## Cоревнование на [kaggle](https://www.kaggle.com/competitions/how-machine-sees)
## Описание задачи
3 класса, машины, самолёты, корабли. \
Есть не большой размеченный датасет. \
Метрика mAP@50\
Пример из датасета:\
<img src="data/datasets/train/images/0a0ae0cb-9a4a-4545-bfa9-206322669db2.jpg" width="200" height="150">
<img src="data/datasets/train/images/0a9da5bd-5d35-497a-a0ec-834b039c420d.jpg" width="200" height="150">
<img src="data/datasets/train/images/0a9947be-f045-4edb-9b69-8d42b6bd46e1.jpg" width="200" height="150">

## Решение
Модель Faster_RCNN, фреймворк Detectron2. \
Модель дообучена на датасете, при обучении применялась аугментация, также данные чистились от других объектов(транспорта), т.к на тестовой выборке их представленно не было