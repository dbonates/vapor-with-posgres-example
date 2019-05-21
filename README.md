# API

## Requests

### **GET** - /api/acronyms/search

#### CURL

```sh
curl -X GET "http://localhost:8080/api/acronyms/search\
?term=What%20The%20Found"
```

#### Query Parameters

- **term** should respect the following schema:

```
{
  "type": "string",
  "enum": [
    "What The Found"
  ],
  "default": "What The Found"
}
```

### **GET** - /api/acronyms/first

#### CURL

```sh
curl -X GET "http://localhost:8080/api/acronyms/first"
```

### **GET** - /api/acronyms/sorted

#### CURL

```sh
curl -X GET "http://localhost:8080/api/acronyms/sorted"
```

### **POST** - /api/acronyms

#### CURL

```sh
curl -X POST "http://localhost:8080/api/acronyms" \
    -H "Content-Type: application/json; charset=utf-8" \
    --data-raw "$body"
```

#### Header Parameters

- **Content-Type** should respect the following schema:

```
{
  "type": "string",
  "enum": [
    "application/json; charset=utf-8"
  ],
  "default": "application/json; charset=utf-8"
}
```

#### Body Parameters

- **body** should respect the following schema:

```
{
  "type": "string",
  "default": "{\"short\":\"OMG\",\"long\":\"Oh My God\"}"
}
```

### **GET** - /api/acronyms

#### CURL

```sh
curl -X GET "http://localhost:8080/api/acronyms"
```

### **GET** - /api/acronyms/2

#### CURL

```sh
curl -X GET "http://localhost:8080/api/acronyms/2"
```

### **PUT** - /api/acronyms/3

#### CURL

```sh
curl -X PUT "http://localhost:8080/api/acronyms/3" \
    -H "Content-Type: application/json; charset=utf-8" \
    --data-raw "$body"
```

#### Header Parameters

- **Content-Type** should respect the following schema:

```
{
  "type": "string",
  "enum": [
    "application/json; charset=utf-8"
  ],
  "default": "application/json; charset=utf-8"
}
```

#### Body Parameters

- **body** should respect the following schema:

```
{
  "type": "string",
  "default": "{\"short\":\"WTF\",\"long\":\"What The Fuck\"}"
}
```

### **DELETE** - /api/acronyms/3

#### CURL

```sh
curl -X DELETE "http://localhost:8080/api/acronyms/3" \
    -H "Content-Type: application/json; charset=utf-8" \
    --data-raw "$body"
```

#### Header Parameters

- **Content-Type** should respect the following schema:

```
{
  "type": "string",
  "enum": [
    "application/json; charset=utf-8"
  ],
  "default": "application/json; charset=utf-8"
}
```

#### Body Parameters

- **body** should respect the following schema:

```
{
  "type": "string",
  "default": "{}"
}
```

## References


