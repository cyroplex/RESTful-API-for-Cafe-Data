
# RESTful-API-for-Cafe-Data

Creating an API for Cafe Data with RestAPI Architecture.


## API Guide

#### All Cafes

```http
  GET /all
```

#### Random Cafe

```http
  GET /random
```

#### Search Cafes by Location

```http
  GET /search?loc={location}
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `loc`      | `string` | **Required**. e.g. Peckham |

#### New Cafe

```http
    POST /add?api-key=TopSecretAPIKey
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `name`      | `string` | **Required**. e.g. Timberyard |

| Body | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `map_url`      | `string` | **Required**. e.g. https://www.google.com/maps/place/TY+Seven+Dials/@51.5128761,-0.1295574,17z/data=!3m1!4b1!4m5!3m4!1s0x487604cd0ed11587:0x3feff9f93e76a986!8m2!3d51.5128761!4d-0.1273687?hl=en-GB |
| `img_url`      | `string` | **Required**. e.g. https://cdn.venuescanner.com/photos/qiUqV/aad7dea72a6fb6f3388ab27ba56b7740.jpg |
| `toilet`      | `boolean` | **Required**. e.g. True |
| `wifi`      | `boolean` | **Required**. e.g. True |
| `sockets`      | `boolean` | **Required**. e.g. True |
| `coffee_price`      | `string` | **Required**. e.g. £3.20 |
| `calls`      | `boolean` | **Required**. e.g. True |
| `seats`      | `string` | **Required**. e.g. 30-40|

#### Update Coffee Price

```http
    PATCH /update-price/3?new_price=£3.80
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `new_price`      | `string` | **Required**. e.g. £3.80 |

#### Delete Cafe By ID

```http
    DELETE /report-closed/1?api-key=TopSecretAPIKey
```
| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `api-key`      | `string` | **Required**. TopSecretAPIKey|



  
