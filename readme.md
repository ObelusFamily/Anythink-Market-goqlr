# Welcome to the Anythink Market repo

To start the app use Docker. It will start both frontend and backend, including all the relevant dependencies, and the db.

Please find more info about each part in the relevant Readme file ([frontend](frontend/readme.md) and [backend](backend/README.md)).

## Development

When implementing a new feature or fixing a bug, please create a new pull request against `main` from a feature/bug branch and add `@vanessa-cooper` as reviewer.

## First setup

1. **[Install docker](https://docs.docker.com/get-docker/)**
2. Verify docker by running the following commands in your terminal:
    ```shell
    docker -v
    docker-compose -v
    ```
3. Start `docker` on your machine:
    ```shell
    sudo systemctl start docker   
    ```
4. To load Anythink's backend and frontend run 
    ```shell
    docker-compose up
    ```
    from the **root directory**
5. Test that **backend** is running by p**ointing your browser** to http://localhost:3000/api/ping
6. Check the **frontend** and make sure it's **connected to the backend**.

   If everything is working properly, you’ll be able to **create a new user** on http://localhost:3001/register