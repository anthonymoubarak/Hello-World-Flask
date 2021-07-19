# Hello-World-Flask
This repository serves as a tutorial on how to save files of a simple Hello World flask application. 

**app.py:** Flask application file that has the python code for running the web application.<br/>
**templates:** A folder that has all html files used by the app.<br/>
**static:** A folder that has all css files used by the app.

**Deploying Application on Heroku** 

Installing prerequisites:<br/>
**pip install flask**<br/>
**pip install git**<br/>
**pip install heroku**<br/>
**pip install gunicorn**<br/>

Download the following repository as a zip file, unzip and move the resulting folder to your desktop: 
https://github.com/anthonymoubarak/Hello-World-Flask.git

1)	Create a free account on https://id.heroku.com/login 
Open terminal/command prompt and run the following commands:
2)	**cd Desktop/Hello-World-Flask-main**
3)	**heroku login**
4)	**heroku create < your_app_name >** (ex: heroku create hello-app)
5)	**pip freeze > requirements.txt**
6)	**touch Procfile**
7)	Enter the following in Procfile:

    **web: gunicorn app:app**

8)	**touch runtime.txt** --> type in this file: python-3.9.0

9) **git init**
   **git add .**<br/>
   **git commit -m “My first commit”**<br/>
   **git push heroku master**<br/>

After running these commands, a URL will be provided that leads to the web app. This URL can be sent to anybody, even if they do not have python, heroku, or any of the libraries used.



