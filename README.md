# Docker-Compose and WordPress with php.ini file.

This is a refactored docker-compose file following the structure of the official exampele from [https://docs.docker.com/compose/wordpress/](https://docs.docker.com/compose/wordpress/).

It addresses the issue of how to **increase the upload limit** and how to change `php.ini` variables within the container. See [https://github.com/docker-library/wordpress/issues/10](https://github.com/docker-library/wordpress/issues/10).


1. Create and configure a `.env` file. (See `.env-example` for an example)
2. Adapt the `wordpress/php.ini` file to your liking.
3. Make sure Docker is running and build the containers by running `docker-compose build`
4. Start the container by running `docker-compose up -d`. You should now be able to bring up wordpress by browsing to `localhost:8000`
