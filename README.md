[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/CdDYOj_4)
# sample-flask-app

This is a simple flask application for practicing continuous deployment.

## Running the application

### Running using Docker

You will need to have [Docker](https://docs.docker.com/engine/install/) installed.

Once you have docker installed, simply run 

`docker compose up` and then go to [http://0.0.0.0:6969](http://0.0.0.0:6969) to see the running web application.

If you want to run it in the background (i.e., you can close the terminal but the site will still be up):

`docker compose up -d`

To shut down the web application, run:

`docker compose down` (or simply ctrl-c if you are running from the terminal, but not in the background)

### Running without docker

1. Install Python (this was tested with python 3.10 but in theory, any version 3.10+ should work)
2. Create virtual environment using `python -m venv .venv`
3. Activate virtual environment  using `source .venv/bin/activate`
4. Install the dependencies `pip install -r requirements.txt`
5. Run `flask run` and then go to [http://127.0.0.1:5000](http://127.0.0.1:5000)

Use ctrl-c to stop the process and shut down the website.

## Relevant tutorials

1. [https://www.digitalocean.com/community/tutorials/how-to-make-a-web-application-using-flask-in-python-3](https://www.digitalocean.com/community/tutorials/how-to-make-a-web-application-using-flask-in-python-3)
2. [https://betterprogramming.pub/create-a-running-docker-container-with-gunicorn-and-flask-dcd98fddb8e0]( https://betterprogramming.pub/create-a-running-docker-container-with-gunicorn-and-flask-dcd98fddb8e0)
