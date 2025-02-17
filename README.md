# Albumy
## Arunaswin Gopinath

*Capture and share every wonderful moment.*

> Example application for *[Python Web Development with Flask](https://helloflask.com/en/book/1)* (《[Flask Web 开发实战](https://helloflask.com/book/1)》).

Demo: http://albumy.helloflask.com

![Screenshot](https://helloflask.com/screenshots/albumy.png)

## Installation

clone:
```
$ git clone https://github.com/arunaswing/albumy_arun.git
$ cd albumy
```
create & activate virtual env then install dependency:
install python version 3.8.20 in the virtual environment.
with venv/virtualenv + pip:
```
$ python -m venv env  # use `virtualenv env` for Python2, use `python3 ...` for Python3 on Linux & macOS
$ source env/bin/activate  # use `env\Scripts\activate` on Windows
$ pip install -r requirements.txt
```
or with Pipenv:
```
$ pipenv install --dev
$ pipenv shell
```
For the ML component, we will be using Azure API:
1. Create an azure account and then setup the Azure Computer Vision API. Key and Endpoint will be generated.
2. Create an .env file and store the endpoint and the key.
```
ENDPOINT="[your personal endpoint]"
KEY="[your personal key]"
```

generate fake data then run:
```
$ flask forge
$ flask run
* Running on http://127.0.0.1:5000/
```
Test account:
* email: `admin@helloflask.com`
* password: `helloflask`

## License

This project is licensed under the MIT License (see the
[LICENSE](LICENSE) file for details).
