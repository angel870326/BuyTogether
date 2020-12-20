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


