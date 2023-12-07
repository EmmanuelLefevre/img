# <span style="color: #005CAB;"><center>BLOG</center></span>
&nbsp;
## <span style="color: #0085FA;"><u>INSTALLATION</u></span>
### <span style="color: #4EABFB;">1. Local</span>
- Install MongoDb Compass and Mongosh shell.  
[MongoDb shell download](https://www.mongodb.com/try/download/shell)  
[MongoDb Compass download](https://www.mongodb.com/try/download/compass)
&nbsp;
- Create database with Mongosh:
```shell
mongosh
```
```shell
use blog
```
```shell
db.createCollection("users")
```
```shell
db.createCollection("articles")
```
[MongoDb create a database documentation](https://www.mongodb.com/docs/manual/core/databases-and-collections/)
***
- Create an authentication
```shell
mongosh
```
```shell
use blog
```
```shell
db.createUser({ user: "Admin", pwd: "nimda", roles: [{ role: "readWrite", db: "blog" }] })
```
[MongoDb create a user documentation](https://www.mongodb.com/docs/manual/tutorial/create-users/)
&nbsp;
#### $${\color{green}Connexion with Mongosh:}$$
```shell
db.auth("Admin","nimda")
```
#### <span style="color: #95cb11;">Connexion with MongoDb VsCode extension:</span>
![Step 1](https://github.com/EmmanuelLefevre/img/blob/main/MongoDb%20VsCode%20extension%20connexion%20step%201.png)
![Step 2](https://github.com/EmmanuelLefevre/img/blob/main/MongoDb%20VsCode%20extension%20connexion%20step%202.png)
***
### <span style="color: #4EABFB;">2. Docker</span>


