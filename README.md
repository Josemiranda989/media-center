# Media Center Docker Compose

Este repositorio contiene un conjunto de servicios Docker configurados con Docker Compose para crear un media center utilizando Plex, Sonarr, Radarr, Jackett, Transmission y Ombi.

<sub>Plex es un servidor de medios que organiza y transmite contenido multimedia, permitiendo acceder a tus películas, series y música desde diferentes dispositivos.

<sub>Sonarr es un gestor de descargas automáticas para series de televisión que busca, descarga y organiza episodios de forma automatizada.

<sub>Radarr es similar a Sonarr, pero está diseñado para películas, automatizando la búsqueda, descarga y organización de tu biblioteca cinematográfica.

<sub>Jackett actúa como un puente entre rastreadores privados de torrents y programas como Sonarr y Radarr, facilitando la búsqueda y obtención de resultados de torrents.

<sub>Transmission es un cliente de torrent que gestiona las descargas de archivos torrent, utilizado por programas como Sonarr y Radarr para obtener contenido multimedia.</sub>

## Requisitos

Asegúrate de tener Docker y Docker Compose instalados en tu sistema antes de comenzar.

- [Docker Installation Guide](https://docs.docker.com/get-docker/)
- [Docker Compose Installation Guide](https://docs.docker.com/compose/install/)

## Pasos para levantar el Media Center

1. **Clona el Repositorio:**

   ```bash
   git clone https://github.com/tu-usuario/media-center-docker.git
   cd media-center-docker
    ```
2. En este caso toda la instalación se crea en la raíz del proyecto, en caso de querer cambiarlo, modifica el valor de la variable de entorno en el archivo `.env`

3. Ejecuta Docker Compose:

    ```bash
   docker-compose up -d
    ```
    Esto iniciará todos los servicios en segundo plano. Puedes acceder a las interfaces web de cada servicio a través de sus respectivos puertos.

4. Accede a los Servicios:

- Plex: http://localhost:32400
- Sonarr: http://localhost:8989
- Radarr: http://localhost:7878
- Jackett: http://localhost:9117
- Transmission: http://localhost:9091
- Ombi: http://localhost:3579
- Ajusta las URL según sea necesario.

¡Listo! Ahora deberías tener un media center funcionando con Docker y Docker Compose.