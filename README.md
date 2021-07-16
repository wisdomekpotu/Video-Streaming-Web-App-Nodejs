# E-learning-Hub
An Open Source E-Learning Upload For University Online Lectures

### Introduction
This project is an Open Source online portal web-application for lecturers of a university to post pre-recorded course lectures for students.



> e-learning web application made using Java 8, Spring Boot, MySql and Materialize

[![GitHub](https://img.shields.io/github/license/donnatto/ez-learning?color=purple)](https://opensource.org/licenses/MIT)
[![GitHub release (latest by date)](https://img.shields.io/github/v/release/donnatto/ez-learning?color=red)](https://github.com/donnatto/ez-learning/releases)
[![GitHub issues](https://img.shields.io/github/issues/donnatto/ez-learning)](https://github.com/donnatto/ez-learning/issues)
![GitHub repo size](https://img.shields.io/github/repo-size/donnatto/ez-learning?color=blue&label=size)
[![GitHub stars](https://img.shields.io/github/stars/donnatto/ez-learning?style=social)](https://github.com/donnatto/ez-learning/stargazers)

[![Ez Learning](https://i.imgur.com/QrXbo6q.jpg)](https://ez-learning.herokuapp.com)

---

### Overview

Fuctionalities:

* Signup.
* Login.
* Upload Lecture Video.
* Delete Lecture Video.


### Tech Stack

Our tech stack will include:

* Nodejs(Express)
* **PostgreSQL** as our database of choice
* **Python3** and **Flask** as our server language and server framework
* **Flask-Migrate** for creating and running schema migrations
* **HTML**, **CSS**, and **Javascript** with [Bootstrap 3](https://getbootstrap.com/docs/3.4/customize/) for our website's frontend


---

## Technologies

Uses [Thymeleaf](https://www.thymeleaf.org/) as the template engine for the Frontend, which was styled using [Materialize](https://materializecss.com/).

The backend is developed in Java 8, using [Spring Boot](https://spring.io/projects/spring-boot) with Spring MVC, Spring JPA and Spring Security dependencies.

It has 2 application profiles, one for development and one for production. The dev profile uses an in memory [H2 Database](https://www.h2database.com/), while the production one uses [MySql](https://www.mysql.com/). Both of them use Sql versioning with [Flyway](https://flywaydb.org/).

The web application is hosted in [Heroku](https://www.heroku.com/), while the MySql database is hosted in a [AWS RDS](https://aws.amazon.com/rds/) instance.

---

### Setup
1. Install the dependencies:
  ```
  $ pip install -r requirements.txt
  ```
2. setup your database in config.py:
  ```
    SQLALCHEMY_DATABASE_URI = 'postgresql://username:password@localhost:5432/databaseName'  

  ```
  in config.py file.
  For Database create at PostgreSQL
  ```
  postgres-# CREATE DATABASE learninghub;
  ```
  You can check the available database list using \l
  ```
  postgres-# \l
  ```
  command to connect/select a desired database
  ```
  postgres=# \c learninghub;
  ```

3. Run the development server:

  ```
  Create Migration 
    $  flask db init

  You can then generate an initial migration
    $ flask db migrate -m "Initial migration."

  Then you can apply the migration to the database:
    $ flask db upgrade
  ```
4. insert data into Course table.
    ```
    $ python courses.py 
    
    ```
    for Default Courses.

5. Run Application:
  ```
  $ flask run
  ```
  Open Browser > http://127.0.0.1:5000/
  
  
  
  ## Contact

Reach out to me at:

- My personal page : [donnatto.com](https://donnatto.com)
- My Blog : [blog.donnatto.com](https://blog.donnatto.com)
- LinkedIn : [linkedin.com/in/donnatto](https://linkedin.com/in/donnatto)
- Instagram : [@donnatto_](https://instagram.com/donnatto_)
- Email : [contact@donnatto.com](mailto:contact@donnatto.com)

---

## License

[MIT License](https://opensource.org/licenses/MIT)

