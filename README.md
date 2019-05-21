
# Examples


## Acronym POST
```bash
curl -X "POST" "http://localhost:8080/api/acronyms" \
     -H 'Content-Type: application/json; charset=utf-8' \
     -d $'{
  "short": "OMG",
  "long": "Oh My God"
}'
```

## Request ALL
```bash
curl "http://localhost:8080/api/acronyms"
```

## Request Single
```bash
curl "http://localhost:8080/api/acronyms/2"
```

## Acronym PUT
```bash
curl -X "PUT" "http://localhost:8080/api/acronyms/3" \
     -H 'Content-Type: application/json; charset=utf-8' \
     -d $'{
  "short": "WTF",
  "long": "What The Fuck"
}'
```

## Acronym DELETE
```bash
curl -X "DELETE" "http://localhost:8080/api/acronyms/3" \
     -H 'Content-Type: application/json; charset=utf-8' \
     -d $'{}'
```

---

## one
```bash
curl "http://localhost:8080/api/acronyms/search?term=What%20The%20Found"
```

## first
```bash
curl "http://localhost:8080/api/acronyms/first"
```

## sorted
```bash
curl "http://localhost:8080/api/acronyms/sorted"
```


