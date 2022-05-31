postgres:
	docker run --name xyz -p 5432:5432 -e POSTGRES_USER=xyz -e POSTGRES_PASSWORD=password -d postgres:14-alpine

createdb:
	docker exec -it xyz createdb --username=xyz --owner=xyz xyz_bank

dropdb:
	docker exec -it xyz psql -U xyz -c  "DROP DATABASE xyz_bank;"