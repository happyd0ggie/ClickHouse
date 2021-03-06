---
toc_priority: 35
toc_title: "\u0411\u0430\u0437\u0430\u0020\u0434\u0430\u043d\u043d\u044b\u0445"
---

# CREATE DATABASE {#query-language-create-database}

Создает базу данных.

``` sql
CREATE DATABASE [IF NOT EXISTS] db_name [ON CLUSTER cluster] [ENGINE = engine(...)]
```

### Секции {#sektsii}

-   `IF NOT EXISTS`

        Если база данных с именем `db_name` уже существует, то ClickHouse не создаёт базу данных и:
        - Не генерирует исключение, если секция указана.
        - Генерирует исключение, если секция не указана.

-   `ON CLUSTER`

        ClickHouse создаёт базу данных `db_name` на всех серверах указанного кластера.

-   `ENGINE`

        - MySQL

            Позволяет получать данные с удаленного сервера MySQL.

        По умолчанию ClickHouse использует собственный движок баз данных.

[Оригинальная статья](https://clickhouse.tech/docs/ru/sql-reference/statements/create/database) 
<!--hide-->
