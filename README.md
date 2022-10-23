Installation and Login of cvat:
1.Install WSL2
2.Download and install Docker Desktop for Windows.
3.Download and install Git for Windows
4.Clone CVAT source code from the GitHub repository using command:
git clone https://github.com/opencv/cvat
and then : cd cvat
5.Run docker containers:
docker-compose up -d
6.Create super user :
winpty docker exec -it cvat_server bash -ic 'python3 ~/manage.py createsuperuser'
7.And finally go to localhost:8080
8.Login with credentials created by the user.
