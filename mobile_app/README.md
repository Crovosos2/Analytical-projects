# Описание проекта
Датасет содержит данные о событиях, совершенных в мобильном приложении "Ненужные вещи". В нем пользователи продают свои ненужные вещи, размещая их на доске объявлений. В датасете содержатся данные пользователей, впервые совершивших действия в приложении после 7 октября 2019 года.<br><br>

Выделить различающиеся по метрикам группы пользователей на основе событий, которые они выполняют в мобильном приложении.<br>

Метрики:
* retention rate, 
* время в приложении, 
* частота совершения событий, 
* конверсия с целевое действие contacts_show

# Описание данных
Датасет **mobile_dataset.csv** содержит колонки:<br>
* `event.time`  — время совершения
* `event.name`  — название события
* `user.id`  — идентификатор пользователя
<br>

Датасет **mobile_sources.csv** содержит колонки:<br>
* `userId`  — идентификатор пользователя
* `source`  — источник, с которого пользователь установил приложение
<br>

Расшифровки событий:
* `advert_open`  — открытие карточки объявления
* `photos_show`  — просмотр фотографий в объявлении
* `tips_show`  — пользователь увидел рекомендованные объявления
* `tips_click`  — пользователь кликнул по рекомендованному объявлению
* `contacts_show`  и  `show_contacts`  — пользователь нажал на кнопку "посмотреть номер телефона" на карточке объявления
* `contacts_call`  — пользователь позвонил по номеру телефона на карточке объявления
* `map`  — пользователь открыл карту размещенных объявлений
* `search_1`  —  `search_7`  — разные события, связанные с поиском по сайту
* `favorites_add`  — добавление объявления в избранное