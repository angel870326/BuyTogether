## Clone and Setup

### Clone

>Clone this repository to my local machine (Mac)

```
cd /Users/angelwang/Desktop
git clone https://github.com/cehsieh12/group-buying.git
```

### Setup Datebase

> Execute MySQL
<br/>系統偏好設定 -> MySQL -> Start MySQL Server
```
/usr/local/MySQL/bin/mysql -u root -p
```

> Create and use database group_buying
```
drop database if exists group_buying;
create database group_buying;
use group_buying;
```

> Quit MySQL
```
quit
```

### Setup App

>**Enter the project folder＊**

```
cd /Users/angelwang/Desktop/group-buying
```

>Install packages via npm

```
npm install
```

>Create config.json file in confile folder (/config/config.json)
```
"development": {
  "username": "root",
  "password": "<YOUR_MySQL_WORKBENCH_PASSWORD>",  // remember to type your password
  "database": "group_buying",
  "host": "127.0.0.1",
  "dialect": "mysql",
  "operatorsAliases": false
}

```

**Create models**

```
npx sequelize db:migrate
```
npx sequelize init

**Activate the server＊**

```
npm start
```

**Find the message for successful activation**

```
> App is running on port 3000!
```
Visit the application on browser with the URL: http://localhost:3000

**Quit the server＊**

```
control+C
```

<br/>

<br/>

## User Interface


|UI|File|
|---|---|
|**Main**|views / main.handlebars <br/>public / stylesheets / main.css|
|**Login & Register**|views / login.handlebars <br/>views / register.handlebars <br/>public / stylesheets / user.css |
|**Groups**|views / index.handlebars <br/>public / stylesheets / main.css <br/>public / stylesheets / index.css <br/>public / stylesheets / bootstrap.css|
|**New Group**|views / new.handlebars <br/>public / stylesheets / new.css <br/>public / stylesheets / todo_form.css <br/>public / stylesheets / main.css <br/>public / stylesheets / bootstrap.css|
|**New Ad**|views / ad.handlebars <br/>public / stylesheets / ad.css|
|**Account**|views / account.handlebars <br/>public / stylesheets / account.css<br/>**Front End Demo: https://youtu.be/ZlYDa-TBWTg **|
|**Detail**|views / detail.handlebars <br/>public / stylesheets / detail.css|
|**- Main Handlers -**|public / stylesheets / bootstrap.css|
|**- Icons -**|public / stylesheets / css / all.css <br/>Source: https://fontawesome.com/license/free|





