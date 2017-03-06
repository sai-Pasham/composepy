# composepy

This is a small we app implementation of a python based web-app in redis server.
Once launched the app can be seen at http://localhost:5000/

Steps :

First create a Dockerfile as mentioned
in Dockerfile :
<li>We are building an image with Python 3.4</li>
<li>Add the current directory "." into the "/code" path of image</li>
<li>Set working directory to /code</li>
<li>Install Python dependencies</li>
<li>Default command is set to Python app.py</li>

Then we will define services in docker-compose.yml file :
<li>We are starting 2 services web and redis</li>
<li>It is built using local Dockerfile</li>
<li>Port 5000 is exposed for use</li>
<li>Directory /code is loaded in web to access </li>

