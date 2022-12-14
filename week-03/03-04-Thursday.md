# Четверг

## Датасет для проекта

Данные доступны по [ссылке](https://disk.yandex.ru/d/kJga-j0b33qbHw)
- более 23 тысяч записей реальных объявлений
- доступные колонки: `['ID  объявления', 'Количество комнат', 'Тип', 'Метро', 'Адрес',
       'Площадь, м2', 'Дом', 'Парковка', 'Цена', 'Телефоны', 'Описание',
       'Ремонт', 'Площадь комнат, м2', 'Балкон', 'Окна', 'Санузел',
       'Можно с детьми/животными', 'Дополнительно', 'Название ЖК',
       'Серия дома', 'Высота потолков, м', 'Лифт', 'Мусоропровод',
       'Ссылка на объявление']`

## Задание

Получить данные, необходимые для моделей машинного обучения. Данные должны быть следующего вида:
- названия колонок **на английском** языке в одно или несколько слов с нижним подчёркиванием
- в каждой колонке должны **отсутствовать** пропущенные значения (NaN, None и т.д.)
- все значения внутри данных должны быть **только** численного типа (int или float)
- должны отсутствовать полные дупликаты объявлений, только **уникальные объявления**

Данные должны быть предоставлены для обучения модели предсказания стоимости **аренды в Москве**. 


## Что можно сделать?

1. "Почистить" данные от NaN 
   - 📝  https://loginom.ru/blog/missing
   - 📝  https://pythobyte.com/python-how-to-handle-missing-dataframe-values-in-pandas-d56af629/
2. Обработать категориальные данные
   - 📝  https://dyakonov.org/2016/08/03/python-категориальные-признаки/
   - 📝  https://habr.com/ru/post/511132/
3. Нормировка
   - 📝  https://habr.com/ru/post/527334/


## Дополнительная информация
- 📝 http://blog.datalytica.ru/2018/04/blog-post.html
- 🐍 [Проект выпускников по оценке рыночной стоимости квартиры](https://github.com/maksimkuragin/Kvocenshik)
