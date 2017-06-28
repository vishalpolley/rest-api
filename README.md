# REST API
This is a simple rest api bulit by using Django REST framework.
## Required Softwares
* [Python](https://www.python.org/downloads/) - Firstly install Python. 
* [Django](https://www.djangoproject.com/download/) - Then install Django.
You are required to install Django version 1.5 or less, as the current code is not valid for higher Django versions.
### To install Django in Ubuntu just run this command in terminal
```
sudo pip install Django==1.5
```

### Running the app
* To run the app first clone the repo.
* Then type the following command in terminal.
```
./manage.py runserver 9000
```

### Working around with api
You can run the following cURL codes in your terminal to test the API.
```
curl http://localhost:9000/api/tasks/
curl -X POST http://localhost:9000/api/tasks/ -d "title=hello world&description=a whole new world"
curl -X PUT http://localhost:9000/api/tasks/1 -d "title=hello world&description=be nice"
curl -X PUT http://localhost:9000/api/tasks/1 -d "title=hello world&description=be nice&completed=True"
curl -X DELETE http://localhost:9000/api/tasks/1
```
