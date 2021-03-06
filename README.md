pip3 freeze > requirements.txt

# Install

### Install python (suguest >3.0)

### Clone and cd to repos
```
git clone 
cd 
```

### Create own virtual enviroment:
```
python3 -m venv env
```
if you using python <3.0, please install virtualenv lib and then:
```
virtualenv env
```
### install package
you can run below cmd to follow this repos
```
pip3 install flask
pip3 install flask-sqlalchemy
pip3 install flask-migrate
pip3 install PyJWT
pip3 install email-validator
pip3 install flask-login
pip3 install Flask-Admin
```
or using install auto from requirements.txt file:
```
pip3 install -r requirements.txt
```
### Edit env
Copy file .flaskenv.sample file and then rename to .flaskenv    
Edit information to correct own enviroment
### Update database
```
flask db init
flask db migrate -m "Update"
flask db upgrade
```


# Using
- run flask:
```
flask run
```
- run shell:
```
flask shell
```

# Structure
- Separat to many BluePrint    
auth: login , logout and authentication user   
errors: handle error    
main: main app   
and add more   
- Config app: in app/__init__.py
- Model for app: in app/model.py  