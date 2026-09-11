# Laboratorio 02

Hoy utilizaremos docker compose para poder desplegar su trabajo. Servicio web y una base de datos

## Stack
API
  - Minimal API
    - Debe retornar un mensaje incluyendo mi nombre
  - Docker

BD
  - PostgreSQL

# Indicaciones

## Configuración Inicial

Antes de levantar los servicios, es necesario crear un archivo `.env` en la raíz del proyecto para definir las credenciales y el mensaje. El archivo debe tener esto:

```env
MESSAGE=Hola, soy Rony Fabrizio Luján Holguín
POSTGRES_USER=postgres
POSTGRES_PASSWORD=mysecretpassword
POSTGRES_DB=db_laboratorio
```

## Comandos

```bash
docker compose up -d
```

## Respuestas

**Tipos de redes en Docker:**
- **Bridge:** Es la red por defecto, aísla los contenedores pero los deja comunicarse entre ellos.
- **Host:** El contenedor usa la red de la máquina directamente.
- **None:** El contenedor no tiene conexión a red.
- **Overlay:** Conecta múltiples demonios de Docker.
- **Macvlan:** Asigna una dirección MAC al contenedor.

**Tipos de volúmenes en Docker:**
- **Volumes:** Gestionados por Docker, son la mejor opción para bases de datos.
- **Bind mounts:** Conectan una ruta específica de tu computadora al contenedor.
- **tmpfs mounts:** Se guardan solo en la memoria RAM.

# Creditos
- Lujan Holguin Rony Fabrizio

![Captura de API](infrasem2.png).