

#DOCKER
docker run --name simplebank --network bank-network -p 8080:8080 -e GIN_MODE=release -e DB_SOURCE="postgresql://root:secret@postgres15:5432/simple_bank?sslmode=disable" simplebank:latest