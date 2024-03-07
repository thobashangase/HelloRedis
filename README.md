# HelloRedis

HelloRedis is a .NET console application example of how to connect, store and retrieve data from Redis, following Ardalis' [blog post](https://ardalis.com/hello-redis-getting-started-with-redis-dotnet/).
 
## Installation and setup
After cloning the repository:

- Download and install the [.NET 8 SDK]().

- Download and install [Docker Desktop]().

- Execute the following command to create and run a Redis container on Docker:

```bash
docker run --name my-redis -p 6379:6379 -d redis
```

- The above will run Redis on port 6379 in daemon mode. 

- Ensure the Redis container is running by executing the following command and confirm that the Redis container is listed:

```bash
docker ps
```

The container will keep running until the user stops it with the below command, where the *container_id* is as per docker ps.

```bash
docker stop {container_id}
```

## Usage
Set your CLI's directory to the directory of the HelloRedis solution and run the application:

```bash
cd HelloRedis
dotnet run
```

## Contributing

Pull requests are welcome. For major changes, please open an issue first
to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License

[MIT](https://choosealicense.com/licenses/mit/)