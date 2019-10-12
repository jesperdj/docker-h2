# H2 Database in Docker

Build the image:

    docker build -t h2 .

Run a container:

    docker run -d -p 8082:8082 -p 9092:9092 --name h2database h2

Access the H2 Console at: http://localhost:8082/

Connect to a database named `test` using JDBC:

- JDBC URL: `jdbc:h2:tcp://localhost/~/test`
- Username: `sa`
- Pasword: (none)
