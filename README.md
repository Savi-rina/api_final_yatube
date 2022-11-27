### Проект API Yatube
Доработан в соответствии с документацией, доступной по ссылке: http://127.0.0.1:8000/redoc/.
Были добавлены недостающие модели в приложении posts, созданы адреса и представления для обработки запросов в приложении api.


### Как запустить проект:
### Клонировать репозиторий и перейти в него в командной строке:
```
git clone https://github.com/Savi-rina/api_final_yatube.git

cd api_final_yatube
```
### Cоздать и активировать виртуальное окружение:
```
python -m venv env
source env/bin/activate
```
### Установить зависимости из файла requirements.txt:
```
python -m pip install --upgrade pip
pip install -r requirements.txt
```
### Выполнить миграции:
```
python manage.py migrate
```
### Запустить проект:
```
python manage.py runserver
```
### Примеры запросов:
### POST-запрос: http://127.0.0.1:8000/api/v1/posts/
Результат:
```
{
  "id": 0,
  "author": "string",
  "text": "string",
  "pub_date": "2019-08-24T14:15:22Z",
  "image": "string",
  "group": 0
}
```
### GET-запрос: http://127.0.0.1:8000/api/v1/posts/{post_id}/comments/
Результат:
```
{
"id": 0,
"author": "string",
"text": "string",
"created": "2019-08-24T14:15:22Z",
"post": 0
}
```
