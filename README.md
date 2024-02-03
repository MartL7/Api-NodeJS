# muAPI

muAPI es una API que proporciona acceso a un catálogo de contenido con detalles sobre películas, series, animes y más.

## Endpoints

### Obtener todo el contenido

```http
GET /content/all

```

### Obtener información a tráves del ID

```http
GET /content/id/:id
```

### Obtener contenido por género

```http
GET /content/genre/:genre
```

### Obtener contenido por tipo (Película, Serie, Anime)

```http
GET /content/type/:type
```

### Ejemplo de uso
curl -X GET http://domain/content/id/1

### Ejemplo del JSON que devuelve la api

```json
[
  {
    "id": 1,
    "title": "Ejemplo de Película",
    "type": "Película",
    "genre": "Acción",
    "poster": "enlace-a-imagen"
  }
]

```