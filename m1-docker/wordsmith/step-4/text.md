Place the following Compose file at the root of the repository:


```yaml
version: "3"
services:
  db:
    build: db
  words:
    build: words
  web:
    build: web
    ports:
    - 8888:80
```

Test the whole app by bringin up the stack and connecting to port 8888.
