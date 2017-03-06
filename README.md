# composepy

This is a small we app implementation of a python based web-app in redis server.
Once launched the app can be seen at http://localhost:5000/

Steps :

First create a Dockerfile as mentioned
in Dockerfile :
<li>We are building an image with Python 3.4
Add the current directory "." into the "/code" path of image
Set working directory to /code
Install Python dependencies
Default command is set to Python app.py</li>

Then we will define services in docker-compose.yml file :
<li>We are starting 2 services web and redis
It is built using local Dockerfile
port 5000 is exposed for use
directory /code is loaded in web to access </li>

