
[Описание](#1)
[Использование](#1)



<a name="1">## Описание:</a> 

**_Web-Сервис сотрудников, сделанный на платформе .Net Core._**

**Сервис должен уметь:**

1. Добавлять сотрудников, в ответ должен приходить Id добавленного сотрудника.
2. Удалять сотрудников по Id.
3. Выводить список сотрудников для указанной компании. Все доступные поля.
4. Выводить список сотрудников для указанного отдела компании. Все доступные поля.
5. Изменять сотрудника по его Id. Изменения должно быть только тех полей, которые указаны в запросе.

**Модель сотрудника:**
```
Employee:
{
  Id int
  Name string
  Surname string
  Phone string
  CompanyId int
  Passport:
  {
    Type string
    Number string
  }
  Department:
  {
    Name string
    Phone string
  }
}
```

**Дополнительно:**

Все методы должны быть реализованы в виде **_HTTP_** запросов в формате **_JSON_**.

**БД:** Любая

**ORM:** Dapper

## Использование: <a name="2">

Запустить контейнеры с `postgreSQL` и `pgAdmin4` кодандой `docker-compose up -d` в корневой папке.

## Стек:

- .NET CORE
- PostgreSQL
- Dapper
- Docker















