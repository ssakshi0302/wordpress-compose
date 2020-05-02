## Requirements
Make sure you have the latest versions of Docker and Docker Compose installed on your machine.

Clone this repository or copy the files from this repository into a new folder. In the docker-compose.yml file you may change the IP address (in case you run multiple containers) or passwords according to your needs.


## Running this project

Just do a simple "docker-compose up" from your directory .

Notes:

The docker volume db_data persists any updates made by WordPress to the database. Learn more about docker volumes

WordPress Multisite works only on ports 80 and 443.


## Bring up WordPress in a web browser

If you are using Docker Machine, you can run the command docker-machine ip MACHINE_VM to get the machine address, and then open http://MACHINE_VM_IP:8000 in a web browser.

If you are using Docker Desktop for Mac or Docker Desktop for Windows, you can use http://localhost as the IP address, and open http://localhost:8000 in a web browser.


## Shutdown and cleanup
The command docker-compose down removes the containers and default network, but preserves your WordPress database.

The command docker-compose down --volumes removes the containers, default network, and the WordPress database.
