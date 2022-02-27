DBPASSWORD=abc123
pg-container-up:
	docker run --rm -it -e POSTGRES_PASSWORD=$(DBPASSWORD) -e POSTGRES_USER=myuser -e POSTGRES_DB=my-db -p 5432:5432 --name pg-n1 postgres:14-alpine3.15

connect-to-container:
	PGPASSWORD=$(DBPASSWORD) psql -h localhost -d my-db -Umyuser

