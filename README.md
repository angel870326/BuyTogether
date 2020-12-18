### Clone

Clone this repository to my local machine (Mac)

```
git clone https://github.com/cehsieh12/group-buying.git
```

### Setup Datebase

**Create and use group_buying MySQL database**
```
/usr/local/MySQL/bin/mysql -u root -p
```
> Run the following code
```
drop database if exists group_buying;
create database group_buying;
use group_buying;
```

### Setup App

**Enter the project folder**

```
cd /Users/angelwang/group-buying
```

**Install packages via npm**

```
npm install
```

**Create config.json file in confile folder**

> /config/config.json
```
"development": {
  "username": "root",
  "password": "<YOUR_MySQL_WORKBENCH_PASSWORD>",
  "database": "group_buying",
  "host": "127.0.0.1",
  "dialect": "mysql",
  "operatorsAliases": false
}

```

**Create models**

> run the following code in the console
```
npx sequelize db:migrate
```

**Activate the server**

```
npm start
```

**Find the message for successful activation**

```
> App is running on port 3000!
```
Visit the application on browser with the URL: http://localhost:3000


