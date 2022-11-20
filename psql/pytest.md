# DB in Pytest run for django

When creating db in pytest run for django, user needs a permission to create db.

```zsh
psql

=> \du -> to list users with permisions

=> ALTER USER your_username CREATEDB;   -> remember about semicolon at the end

=> \du -> double check the permissions
```

In `pytest.ini` use:

```
addopts = --showlocals --color=yes --durations 5 -vv --reuse-db
```

Use `--create-db` to force db recreation
