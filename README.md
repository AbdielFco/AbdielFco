# 📌 API de Publicaciones

Bienvenido a la API de Publicaciones. Aquí puedes gestionar publicaciones, usuarios, likes, vistas y comentarios de manera sencilla. 🚀

---

## 🌍 Rutas Principales

### 📄 Artículos (Posts)
| Método | Ruta | Descripción |
|--------|------|-------------|
| GET | `/api/articles` | Obtener todos los posts |
| POST | `/api/articles/search` | Buscar un post por ID |
| POST | `/api/articles/new` | Crear un nuevo post |
| DELETE | `/api/articles/delete/{id}` | Eliminar un post |

### 👍 Likes
| Método | Ruta | Descripción |
|--------|------|-------------|
| POST | `/api/articles/like/new` | Crear un like |
| DELETE | `/api/articles/like/delete/{id}` | Eliminar un like |
| POST | `/api/articles/like` | Verificar si un usuario ha dado like |

### 👀 Vistas
| Método | Ruta | Descripción |
|--------|------|-------------|
| POST | `/api/articles/view/new` | Registrar una nueva vista |

### 💬 Comentarios
| Método | Ruta | Descripción |
|--------|------|-------------|
| GET | `/api/articles/comment` | Obtener todos los comentarios |
| POST | `/api/articles/comment/new` | Crear un nuevo comentario |

### 👤 Usuarios
| Método | Ruta | Descripción |
|--------|------|-------------|
| GET | `/api/users` | Obtener todos los usuarios |
| POST | `/api/users/login` | Verificar usuario |
| POST | `/api/users/register` | Registrar un usuario |
| DELETE | `/api/users/delete/{id}` | Eliminar un usuario |

---

## 🔍 Ejemplos de Uso

### 📝 Obtener todos los posts
```http
GET http://localhost:4000/api/articles
```

### 🔍 Buscar un post por ID
```http
POST http://localhost:4000/api/articles/search
Content-Type: application/json

{
    "id": "1739316258"
}
```

### 🆕 Crear un nuevo post
```http
POST http://localhost:4000/api/articles/new
Content-Type: application/json

{
    "id": "{{$timestamp}}",
    "title": "Nuevo Post",
    "date": "{{$timestamp}}",
    "description": "Descripción del post",
    "content": "Contenido del post",
    "image": "",
    "author_id": "1"
}
```

### ❌ Eliminar un post
```http
DELETE http://localhost:4000/api/articles/delete/{{id}}
```

### 👍 Dar like a un post
```http
POST http://localhost:4000/api/articles/like/new
Content-Type: application/json

{
    "id": "{{$timestamp}}",
    "post_id": "1739316258",
    "author_id": "1",
    "date": "{{$timestamp}}"
}
```

### 🏁 Registro de usuario
```http
POST http://localhost:4000/api/users/register
Content-Type: application/json

{
    "id": "{{$timestamp}}",
    "name": "Yeremia",
    "password": "12345678",
    "email": "yeremy@gmail.com"
}
```

---

## 🛠 Requisitos y Configuración
- Asegúrate de que el servidor está corriendo en `http://localhost:4000`
- Utiliza herramientas como [Postman](https://www.postman.com/) o [Restclient](http://restclient.net/) para probar las solicitudes

🚀 ¡Ahora estás listo para interactuar con la API! 🎉

