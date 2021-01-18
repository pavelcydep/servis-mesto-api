# Проект Mesto фронтенд + бэкенд 

## Описание:
Проэктная работа создана с целью закрепить познания в Express.js на практике. Сервер предоставляет статику сайта, а также отвечает на Get запросы.

## Функционал: 
### GET запросы:
- Запрос на `localhost:3000/users` вернет список всех пользователей из базы **mestodb**
- Запрос на `localhost:3000/cards` вернет список всех карточек всех пользователей из базы **mestodb**
- Запрос на `localhost:3000/cards/:userId` вернет конкретного пользователя с переданным после **/users** идентификатором

### POST запросы:
- Создание пользователя
Запрос на `localhost:3000/users`
В теле POST-запроса на создание пользователя необходимо передать **JSON**-объект с тремя полями:
```sh
{
    "name": "Имя пользователя",
    "about": "Описание",
    "avatar": "Ссылка на аватар пользователя"
}
```
- Создание карточки
Запрос на `localhost:3000/cards`
В теле POST-запроса на создание карточки необходимо передать **JSON**-объект с двумя полями:
```sh
{
    "name": "Место",
    "link": "Ссылка на фотографию места",
}
```
### DELETE запросы:
- Удаление карточки по её id
Запрос на `localhost:3000/cards/:cardId` удаляет карточку с переданным после **/cards** идентификатором

## Технологии:
* Express.js
* Node.js


## Запуск проекта:

`npm run start` — запускает сервер   
`npm run dev` — запускает сервер с hot-reload

