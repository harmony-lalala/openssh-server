# OpenSSH Server with Git

## Starting the server

1. Create a file `authorized_keys` in `config` folder

2. Checkout the repos you need into `repos` folder:

    ```
    git clone --bare <repo.git>
    ```

3. Start the server:

    ```
    docker-compose up -d
    ```

## Stopping the server

```
docker-compose stop
```