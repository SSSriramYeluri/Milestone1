Installation and Login of cvat:
Install WSL2
Download and install Docker Desktop for Windows.
Download and install Git for Windows
Clone CVAT source code from the GitHub repository using command:
    git clone https://github.com/opencv/cvat
    and then : cd cvat
Run docker containers:
    docker-compose up -d
Create super user :
    winpty docker exec -it cvat_server bash -ic 'python3 ~/manage.py createsuperuser'
And finally go to localhost:8080
Login with credentials created by the user.
