# standard start procedures

## working with existing project:

```python -m venv venv```
to establish virtual environment (the second venv is your local environment suggested name)

```venv/Scripts/activate```
to activate virtual environment locally (where venv is your local environment name)

```pip install -r requirements.txt```
to install all the requested modules and packages

## starting new project:

```python -m venv venv```
to estabilsih virtual environment (where the second venv is your local environment suggested name)

```venv/Scripts/activate```
to activate virtual environment locally

```pip install flask```
to install flask microframework

```pip install python-dotenv```
if you are planning to work with .env file. And believe me you will :)

```pip install psycopg2```
if you are planning to work with databases (such as MySQL or Postreg)

```pip install bcrypt```
if you are planning to work/hash passwords

and finally...
```pip freeze > requirements.txt```
to create __requirements.txt__ file including all needed modules and packages list.
Remember to use this command every time you are adding a new module to the project.

## AND FOR BOTH:

```$env:FLASK_APP="filename.py"```
where filename.py is your main application python file to enable ```flask run``` command.

```$env:FLASK_ENV="development"```
to switch the current flag to development mode which has a standard debugger mode on

```$env:FLASK_DEBUG="1"```
ONLY if debugger won't be active as a standard

REMEMBER TO SWITCH THE FLAG TO __"production"__ BEFORE DEPLOYING THE PROJECT.

---
_Last update: 5 June 2023_ 