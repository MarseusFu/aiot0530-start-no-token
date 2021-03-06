# AIoT Github

## Lecture 15: IoT Flask Web (deploy to heroku)

### step 1 : Clone this github

### step 2 : install some package


```python
pip insall gunicorn   
Flask==2.0.1 
Jinja2==3.0.1 
psycopg2 
sklearn 
pandas  
numpy 
```

### step 3: add an heroku postgredb

* register heroku account
* go to dashboard
* new an app
* go to resource and add-on an Heroku postgredb

### step 4: login to heroku pstgredb using HeidiSQL


```sql
myserver ="<fill-in-Heroku-Postgredb-DB-sever>"
myuser="<fill-in-Heroku-Postgredb-DB-user>"
mypassword="<fill-in-Heroku-Postgredb-DB-pwd>"
mydb="<fill-in-Heroku-Postgredb-DB-db>"

```
### step 5: import postgredb (in db/postgre.db)


### step 6: setting db in app.py


```sql
myserver ="<fill-in-Heroku-Postgredb-DB-sever>"
myuser="<fill-in-Heroku-Postgredb-DB-user>"
mypassword="<fill-in-Heroku-Postgredb-DB-pwd>"
mydb="<fill-in-Heroku-Postgredb-DB-db>"

```
### step 7: testing locally by running python app.py

### step 8: deploy to github (new private github repositoy)

delete .git and git remote add origin master github.com/xxxxx


### step 9: Heroku deploy from github

### step 10: Complete

Sample link 1:
https://awinlab-aiot.herokuapp.com/

Sample link 2: 
https://aiot0529.herokuapp.com/




# My Version:
### step 3 add an heroku postgredb:
![image](https://i.imgur.com/A7rIDBh.png)
### step 4 login to heroku pstgredb using HeidiSQL:
![imgae](https://i.imgur.com/x7aWb8b.png)
### step 5 import postgredb (in db/postgre.db):
![imgae](https://i.imgur.com/uOSbCWt.png)
### step 6 setting db in app.py:
![image](https://i.imgur.com/jkAynuZ.png)
因為發現此方法不可行(一段時間後會需要maintain database導致heroku那個app link不能用)，故用以下作法
先上heroku找到你app，setting>config vars
![image](heroku_appsetting.jpg)
在照以下修改程式碼
![image](maintain_db_1.jpg)
![image](maintain_db_2.jpg)
### step 7 to 9 follow teacher's step
## Result :
setRandom:<br>
![image](https://i.imgur.com/OHxMj04.png)<br>
CallAI:<br>
![image](https://i.imgur.com/kaQqI3q.png)<br>
**‧** Heroku - [Link](https://aiot0531-test2.herokuapp.com/)
