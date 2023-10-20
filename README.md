# go-web-service-gin
https://go.dev/doc/tutorial/web-service-gin


## Run the app server
From root `go run .`

## Get Albums
```
curl http://localhost:8080/albums \
    --header "Content-Type: application/json" \
    --request "GET"
```

## Get Album
```
curl http://localhost:8080/albums/2
```

## Post Album
```
curl http://localhost:8080/albums \
    --include \
    --header "Content-Type: application/json" \
    --request "POST" \
    --data '{"id": "4","title": "The Modern Sound of Betty Carter","artist": "Betty Carter","price": 49.99}'
```