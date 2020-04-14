# OpenSSH Server with Git

## Starting the server

1. Create a `.ssh` folder inside `config` folder

    ```
    mkdir -p ./config/.ssh
    ```

2. Create an `authorized_keys` file and fill it with public keys.

    ```
    touch ./config/.ssh/authorized_keys
    ```

3. Checkout the repos you need into `repos` folder:

    ```
    git clone --bare <repo.git>
    ```

4. Start the server:

    ```
    docker-compose up -d
    ```

## Stopping the server

```
docker-compose stop
```