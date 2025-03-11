#### untuk melakukan migration ke database

```
migrate -database "mysql://root@tcp(localhost:3306)/belajar_golang_database_migration" -path db/migrations up
```

#### untuk melakukan rollback migration

```
migrate -database "mysql://root@tcp(localhost:3306)/belajar_golang_database_migration" -path db/migrations down
```