# husky-api

# Running on local environment
```bash
source husky/bin/activate
```

```bash
cd src/
uvicorn main:app --host 0.0.0.0 --port 8000
```

# Running on docker container
Build the docker image
```bash
docker build -t husky-api ./src
```

Run the container with 8000 port exposed
```bash
docker run -p 8000:8000 husky-api
```