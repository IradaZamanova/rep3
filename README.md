# GitHub

Описание проекта : [Сайт GitHub](https://github.com/)

Назначение этой Postman коллекции заключается в автоматизации, тестировании и документировании API запросов.


## Использование
1. Установите [Postman](https://www.postman.com/downloads/) на свой компьютер
2. Скачайте текущую коллекцию.
3. Импортируйте коллекцию в Postman.
4. В Autorization добавьте Bearer Token - ваш токен GitHub.


## Переменные среды
- token - ваш токен GitHub.
- R - название вашего репозитория.
- IZ - ваш ник на GitHub.
- GitHub - api GitHub: https://api.github.com/
- ISS - issues
- REP - repos


## Описание запросов
   1. **Создание issue:**
   - Описание: Создает новую задачу в репозитории GitHub.
   - Путь: /repos/{owner}/{repo}/issues
   - Метод: `POST`
   2. **Получение списка задач:**
   - Описание: Возвращает список задач из репозитория GitHub.
   - Путь: /repos/{owner}/{repo}/issues
   - Метод: `GET`
   3. **Изменение названия задачи:**
   - Описание: Изменяет название существующей задачи в репозитории GitHub.
   - Путь: /repos/{owner}/{repo}/issues/{issue_number}
   - Метод: `PATCH`
  4. **Удаление задачи:**
   - Описание: Удаляет существующую задачу из репозитория GitHub.
   - Путь: /repos/{owner}/{repo}/issues/{issue_number}/lock
   - Метод: `DELETE`

В этих запросах 

-owner - ваш ник на Github

-repo - название вашего репозитория
