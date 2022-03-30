I created this project to become further understand how to create a docker image using docker compose yml file and Dockerfile.  

## Getting Started

I started the project with the manage.py file which is the content of the project which will display on the webpage.  Using the Dockerfile and the docker-compose.yml file, I created the image necessary for the project.  The requirement.txt will list the packages needed for the project.   The packages are installed on the image, not the local environment.

### DockerFile
1. Fetch the Python 3 image.
2. Provide the environmental variable to not write byte code.
3. Provide the environmental variable to not buffer.
4. Establish the working directory.
5. Copy the requirements.txt of the local environment to the image environment.
6. Run PIP to install the requirements listed in the image.
7. Copy the local file to the image.

### docker-compose.yml
1. Run Docker Version 3.9
2. Run the 1st of 2 services: Web Service
3. Build using the current directory.
4. Build using the listed volumes for data.
5. Build using the listed ports.
6. Build with the postgress name, user and password.
7. Establish the db for the environment

### Database
1. Fetch the Postgres image.
2. Connect the data volumns
3. Use the web environment details for the database.