# H2 Database in Docker

Build the image:

    docker build -t jesperdj/h2 .

Or pull it from Docker Hub:

    docker pull jesperdj/h2

Run a container:

    docker run -d -p 8082:8082 -p 9092:9092 --name exampledb jesperdj/h2

Check the logs:

    docker logs -f exampledb

Access the H2 Console at: http://localhost:8082/

Connect to a database named `test` using JDBC (the database will automatically be created if it does not yet exist):

- JDBC URL: `jdbc:h2:tcp://localhost/test`
- Username: `sa`
- Password: (none)
