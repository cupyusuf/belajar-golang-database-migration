#### untuk melakukan migration ke database

```
migrate -database "mysql://root@tcp(localhost:3306)/belajar_golang_database_migration" -path db/migrations up
```
#### untuk melakukan migration ke versi tertentu
```
migrate -database "mysql://root@tcp(localhost:3306)/belajar_golang_database_migration" -path db/migrations up 2
```

#### untuk melakukan rollback migration

```
migrate -database "mysql://root@tcp(localhost:3306)/belajar_golang_database_migration" -path db/migrations down
```

#### untuk membuat migration baru

```
migrate create -ext sql -dir db/migrations create_table_first
migrate create -ext sql -dir db/migrations create_table_second
migrate create -ext sql -dir db/migrations create_table_third
```
