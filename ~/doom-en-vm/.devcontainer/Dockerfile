# Usa Ubuntu 20.04 como base
FROM ubuntu:20.04

# Evita interacción manual durante la instalación de paquetes
ENV DEBIAN_FRONTEND=noninteractive

# Instala dependencias necesarias para correr Doom
RUN apt-get update && apt-get install -y \
    chocolate-doom \
    x11-apps \
    libx11-6 \
    && apt-get clean

# Si fuera necesario descargar el archivo WAD (comentado)
# RUN mkdir /root/.local/share/doom && \
#     wget -O /root/.local/share/doom/DOOM1.WAD https://example.com/doom1.wad

# Comando por defecto al iniciar el contenedor
CMD ["chocolate-doom"]
