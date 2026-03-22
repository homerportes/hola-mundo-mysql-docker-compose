# Hola Mundo + MySQL con Docker Compose

Aplicacion web en Python (Flask) que responde "Hola Mundo" y verifica conexion a una base de datos MySQL.

## Estructura

- `src/app.py`: aplicacion Flask
- `src/requirements.txt`: dependencias
- `src/Dockerfile`: imagen del servicio app
- `docker-compose.yml`: orquestacion de servicios app + mysql

## Ejecutar

```bash
docker compose up --build
```

Luego abre:

- http://localhost:5000

Respuesta esperada (JSON):

```json
{
  "message": "Hola Mundo",
  "mysql_connected": true,
  "mysql_status": "Conexion a MySQL exitosa"
}
```
