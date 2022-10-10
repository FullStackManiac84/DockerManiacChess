# DockerManiacChess
A Chess API via Docker

To Install Game via Docker Container:

1) Clone the DockerManiacChess
2) Start up a docker daemon
3) In command prompt, issue the following command : "docker build -t maniacchessapp . "
4) Then issue the following command in prompt : "docker run -p 80:8080 maniacchessapp"
5) Open browser and navigate to http://localhost/Test5/PlayerBegin.jsp

To Get the Save and Retrieve Buttons Functioning:

1) Issue command from terminal : "docker exec -it <container-id> bash" where <container-id> corresponds
   to the instance of maniacchessapp (you can use "docker ps" to discover this)
2) Issue command "apt-get update"
3) Issue command "apt-get install mongodb"
4) Once mongo is installed successfully, go to the root directory ("cd ~")
5) Issue command "mkdir -p data/db"
6) Go into directory root directory /usr/bin, and then type "mongo" in terminal. The mongo instance should
   now be running.
7) That's it! You should now be able to save and retrieve games.
