# Junior test task

## Backend
Write a REST FULL service on **NodeJs** **Koa** which will process GET, POST, PUT, DELETE requests.

**MySQL** has a table of reports:
```
CREATE TABLE `error_reports` (
    `id` INT (10) UNSIGNED NOT NULL AUTO_INCREMENT,
    `host` VARCHAR (255) NOT NULL,
    `code` INT (10) UNSIGNED NOT NULL,
    `message` MEDIUMTEXT NOT NULL,
    `created_at` DATETIME NULL DEFAULT,
    `updated_at` DATETIME NULL DEFAULT,
    PRIMARY KEY (`id`)
)
COLLATE = 'utf8_general_ci'
ENGINE = InnoDB;
```

Need to:
1) create a data model for a table using sequelize

2) handle the relevant REST requests:

- GET - returns a list of reports
- GET with specified id - returns a specific record from reports
- POST - creates a new record in reports
- PUT - updates an existing record in reports
- DELETE - deletes the record from reports

The data return format is JSON

3) Add basic validation (all required fields are required)

## Frontend

Write on **Angular** (v7-v8) a simple application that will show a list of reports, each report can be edited, deleted. Above list - button for add a new report. The frontend must use the REST service.

## Optional (like a bonus)
Push code to GitHub + deploy to Heroku and send link
