When creating db in pytest run for django, user needs a permission to create db.

```zsh
psql

=> \du -> to list users with permisions

=> ALTER USER your_username CREATEDB;   -> remember about semicolon at the end

=> \du -> double check the permissions
```
