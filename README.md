# hh_pet
Это самостоятельный проект по исследованию вакансий на сайте hh.ru.
Работа проводилась в несколько этапов:
- Подготовка инфраструктуры: на виртуальной машине установка сервера PostgreSQL + pgAdmin, создание отдельных пользователей и базы данных.
- Сбор, первичная обработка и подготовка к загрузке в БД PostgreSQL данных при помощи Python.
- Создание таблиц в PostgreSQL для подготовленных данных.
- Загрузка данных в таблицы.
- Созданием отчета в PowerBI. Ссылка на отчет: https://app.powerbi.com/view?r=eyJrIjoiZjI1NzFiMDAtMTRjNy00ODliLWJhZDMtZTZmY2U0ZTA2OGUxIiwidCI6IjFkOTBlZjk5LTE0ZTMtNDQxNC04MTQwLTk1N2IwMDBiOTBjNiJ9

В данном репозитории находятся файлы:
hh_professions.ipynb
  Создание списка профессий и категорий по которым проводились исследования. Также производилась подготовка поисковых запросов к API на hh.ru.

hh_spec_cities.ipynb
  Подготовка информации по городам, используемым на hh.ru, и дополнение этой информации по данным Росстат (средняя зп по регионам и численности населения).

hh_professions.ipynb
  Загрузка данных через API hh.ru. Предобработка и загрузка в БД.
  
hh_tfidf.ipynb
  Очистка и лемматизация слов из описания и ключевых навыков вакансий. Расчет метрики TF-IDF - важности ключевых навыков и слов из описания к вакансиям. В последствии использовалась только важность ключевых навыков.
