# API yatube

## Описание

API соцсети, 9й спринт ЯП

## Установка

Клонировать репозиторий
```
git clone <diz_progect>
```

В папке с проектом установить и активировать виртуальное окружение
```
python -m venv venv
source venv/Scripts/activate
```

Установить зависимости
```
pip install requirements.txt
```


## Функционал

По адресу можно:

```
api/v1/posts/
```
Запрашивать все посты или отправлять свой (если зареган)
GET и POST, соответственно

```
api/v1/posts/{id}/
```
Получить доступ к отдельному посту
GET
А если пост ваш, то можно и редактировать, и удалять
PUT, PATCH, DELETE

```
api/v1/posts/{post_id}/comments
```
Получить доступ к коментариям поста
GET
Добавлять комментарий (для зарегистрированных)
POST
А если коммент ваш, то можно и редактировать, и удалять
PUT, PATCH, DELETE

```
api/v1/groups/
```
Получить доступ к списку сообществ
GET

```
api/v1/groups/{id}
```
Получить доступ к интересующему сообществу
GET

```
api/v1/follow/
```
Подписаться на интересующего автора (для зарегистрированных)
POST
Посмотреть свои подписки
GET

```
api/v1/jwt/create/
```
Получить желанный JWT-token
POST
(не забудьте передать данные пользователя)

```
api/v1/jwt/refresh/
```
Обновить Ваш JWT-token
POST

```
api/v1/jwt/refresh/
```
Проверить Ваш JWT-token
POST

## Автор
Дьячков Владислав