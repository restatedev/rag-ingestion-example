
# Setup ollama locally to download the model 

```bash
mkdir ollama/
```

```
docker-compose pull
docker-compose build
docker-compose up
```

From a seperate terminal, download the embedding model.
We are using mxbai-embed-large.


```bash
curl http://localhost:11434/api/pull -d '{ "name": "mxbai-embed-large" }'
```

# All done, now you can go and upload files to this bucket!

* Minio console [http://localhost:9001/browser/docs](Minio)
* Qdrant [http://localhost:6333/dashboard#/collections](Qdrant)


# To teardown

```
docker-compose down --remove-orphans
```

