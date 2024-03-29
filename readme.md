If you're looking to securely download movies via Magnet links without worrying about catching viruses, then this project is for you. Thanks to two Docker containers, we can safely download films using Qbittorrent first and then visualize them on a secure website.

Using Docker containers ensures virus-free downloads because the downloaded files have no access to the host PC; only the Docker containers have access.

## The installation
1. Make sure you have Docker installed.
2. Launch the docker-compose.yml file using the command: `docker compose up`.
3. After that, you can use the 2 provided bash scripts to easily start or stop all services (on Windows)

## How to use all of it:
To download movies, you need to obtain their Magnet link and then visit `localhost:8080` to download the film using Qbittorrent web app. Upon the first connection, you'll need to use `admin` as the username and the password provided when launching the command `docker compose up` for the first time.
Once the download is complete, you can watch the movie by navigating to `localhost:8000`, where you can browse through your downloaded files to find the movie you downloaded.
