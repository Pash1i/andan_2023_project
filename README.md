# andan_2023_project
Проект для курса по анализу данных на питоне в ВШЭ 2023

Изначально мы заявляли, что будем анализировать твиты Илона Маска и их влияние на котировки акций компании тесла. Но во время сбора данных мы столкнулись с проблемой: твиттер архивирует старые твиты. Из-за этого с одного аккаунта получается собрать только около 600 последних твитов. Для Илона Маска, который является очень активным пользователем твиттера (всего у него около 25 тысяч публикаций) это означает, что получится собрать данные только до ноября 2022 года. Бирживые котировки доступны только для будних и непраздничных дней. В итоге, у нас оставалось порядка 250 наблюдений (замэтченных твиттов и котировок). Мы посчитали, что этого недостаточно для хорошего проекта, поэтому мы решили сменить тему проекта. Несистематизированные (и незаконченные) результаты работы с твитами Илона Маска можно найти по [ссылке](https://github.com/Pash1i/andan_2023_project/tree/do_not_need).

## Новая тема проекта: Анализ постов в вк-группе [dying](https://vk.com/ldyingl)

Мы решили проанализировать посты в сообществе dying - уникальной группе вк, просуществовавшей с ноября 2014 года по август 2015 года. В ней публиковались в основном небольшие текстовые посты кринжово-сопливо-подростково-я-не-такая/такой-как-все содержания. Для того, чтобы воплотить нашу задумку в жизнь, мы собрали ВСЕ посты, опубликованные в данной группе. Получилось около девяти с половиной тысяч штук. Сбор данных был реализован с помощью библиотеки Selenium. 

-  Код, собирающий посты, количество лайков и репостов в группе dying cмотри [здесь](https://github.com/Pash1i/andan_2023_project/blob/main/scrapping_dying.ipynb).

- Первичная обработка текстовых данных лежит [тут](https://github.com/Pash1i/andan_2023_project/blob/main/data_preprocessing.ipynb)
		
Также мы собрали [данные о погоде](https://github.com/Pash1i/andan_2023_project/blob/main/проект%20weather.ipynb) (там же смотри описание признаков) в дни активности паблика dying, чтобы проанализировать, что лучше предсказывает количество лайков на постах паблика: погода в Москве в день публикации или все-таки содержание поста. В это довольно трудно поверить, но содержание постов предсказывает количество лайков немного лучше. Машинное обучение лежит [здесь](https://github.com/Pash1i/andan_2023_project/blob/main/EDA_and_hypothesis_testing.ipynb).

[Там же](https://github.com/Pash1i/andan_2023_project/blob/main/EDA_and_hypothesis_testing.ipynb) лежит визуальный анализ имеющихся данных и тестирование пары гипотез.
