FROM ubuntu:20.04

# Evita interacción en la instalación
ENV DEBIAN_FRONTEND=noninteractive

# Instala dependencias
RUN apt-get update && apt-get install -y \
    chocolate-doom \
    x11-apps \
    libx11-6 \
    && apt-get clean

# Copiamos un WAD por defecto si no se monta otro (opcional)
# RUN mkdir /root/.local/share/doom && wget -O /root/.local/share/doom/DOOM1.WAD https://example.com/doom1.wad

# Comando por defecto
CMD ["chocolate-doom"]


Usa Ubuntu 20.04 como base.

Instala Chocolate Doom.

Prepara el contenedor para ejecutar el juego con interfaz gráfica si usas X11 en tu host.

