# Setup

```
$ curl https://sh.rustup.rs -sSf | /bin/bash -s -- -y --default-toolchain nightly
```

# Run Web server

```
$ cargo run
```

# Usage

## Get todo list

```
$ curl -i http://localhost:8000/todos
```

## Get todo item

```
$ curl -i http://localhost:8000/todos/1
```

## Post todo

```
$ curl -i -H "Content-Type: application/json" -X POST -d '{"id": 100, "title":"Read this book", "description": "http://shop.oreilly.com/product/0636920040385.do", "done": false}' http://localhost:8000/todos
```
