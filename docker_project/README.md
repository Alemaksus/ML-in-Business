### Итоговый проект курса "Машинное обучение в бизнесе"

Автор: Алекс Максаков

Стек: 

* ML: sklearn, pandas, numpy
* API: flask
* Данные: Kaggle - (https://www.kaggle.com/arashnic/hr-analytics-job-change-of-data-scientists)

Задача: предсказать вероятность смены работы по характеристикам сотрудника. Бинарная классификация

Используемые признаки:


* city_development_index (float)
* training_hours (int)
* gender (text)
* education_level (text)
* enrolled_university (text)
* major_discipline (text)
* experience (text)
* relevent_experience (text)
* last_new_job (text)
* company_size (text)
* company_type (text)
* city (text)

Преобразования признаков: OneHotEncoder, CatBoostEncoder, кастомный энкодер для поля 'experience'

Модель: CatBoost

#### Клонируем репозиторий

'''
$ git clone https://github.com/Alemaksus/ML-in-Business

$ cd docker_project
'''

#### Запускаем контейнер

$ docker run -d -p 8180:8180 -p 8181:8181 -v <C:\Coding\Data Science\ML in Business\docker_project\app>:/app/app/ML-in-Business/docker_project/app/training_files/

$ docker-compose up -d



