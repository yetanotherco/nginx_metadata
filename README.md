# nginx_metadata

To run the server use the following command

```
docker run -d -p 8080:80 --name nginx-json-server \
  -v "./conf.d:/etc/nginx/conf.d:ro" \
  -v "./html:/usr/share/nginx/html:ro" \
  nginx:latest
```

This will expose the following endpoints

- http://localhost:8080/data.json
- http://localhost:8080/logo.png
