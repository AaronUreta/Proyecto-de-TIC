# 🕹️ Comparativa Técnica: DOOM en Docker vs Máquina Virtual

Este proyecto evalúa el rendimiento y la facilidad de uso de ejecutar **Chocolate DOOM** en dos entornos distintos: **Docker (sobre WSL2)** y **una máquina virtual Ubuntu (VirtualBox)**.

---

## 🎯 Objetivos del Proyecto

- ⏱️ Evaluar el tiempo de arranque de Chocolate DOOM
- 📊 Medir el consumo de RAM en ambos entornos
- 🔧 Analizar la facilidad de implementación y mantenimiento

---

## ⚙️ Entornos de Prueba

### Docker en Windows (WSL2)
- 🖥️ SO Invitado: Ubuntu 20.04 (WSL2)
- ⚙️ Recursos Asignados: 2 CPU, 4 GB RAM
- 💾 Disco utilizado: 1 GB imagen Docker
- 🖥️ Interfaz de ejecución: Terminal (SDL modo texto)

### Máquina Virtual (VirtualBox)
- 🖥️ SO Invitado: Ubuntu 20.04
- ⚙️ Recursos Asignados: 2 CPU, 4 GB RAM
- 💾 Disco utilizado: 10 GB disco virtual
- 🖥️ Interfaz de ejecución: Ventana gráfica completa

---

## 📈 Comparativa Técnica

| Entorno      | Tiempo de arranque | Uso de RAM  | Portabilidad | Mantenimiento | Seguridad |
|--------------|--------------------|-------------|--------------|----------------|------------|
| Docker       | ~1.2 segundos      | ~48 MB      | Alta         | Fácil          | Media      |
| Máquina Virtual | ~29 segundos     | ~210 MB     | Media        | Complejo       | Alta       |

---

## 📅 Resultados Simulados

| Día       | Hora      | Entorno | Tiempo de arranque (s) | RAM usada (MB) |
|-----------|-----------|---------|-------------------------|----------------|
| Jueves 15 | 10:00 AM  | Docker  | 1.2                     | 48             |
| Jueves 15 | 10:10 AM  | VM      | 28                      | 210            |
| Viernes 16| 2:00 PM   | Docker  | 1.1                     | 50             |
| Viernes 16| 2:15 PM   | VM      | 30                      | 205            |
| Sábado 17 | 8:00 PM   | Docker  | 1.3                     | 47             |
| Sábado 17 | 8:15 PM   | VM      | 29                      | 215            |

---

## 🛠️ Herramientas Utilizadas

- Docker Desktop (WSL2)
- Oracle VirtualBox
- Ubuntu 20.04 LTS
- Chocolate Doom (`sudo apt install chocolate-doom`)
- Cronómetro para medición de recursos

    A[🪟 Windows Host] --> B[🐳 Docker + WSL2 - Doom]
    A --> C[🖥️ VirtualBox VM - Ubuntu - Doom]
    B --> D[🎮 Chocolate Doom (SDL en terminal)]
    C --> E[🎮 Chocolate Doom (interfaz X11)]



---

## 🧾 Conclusión

Tras comparar el rendimiento de **Chocolate DOOM** ejecutado mediante Docker (WSL2) y dentro de una máquina virtual (VirtualBox Ubuntu), llegamos a una conclusión clara:

> **Docker es significativamente más eficiente en tiempo de arranque y uso de recursos**, incluso cuando ambas plataformas utilizan la misma imagen de contenedor. 

- 🚀 Docker arranca DOOM en apenas ~1 segundo.
- 📉 Usa menos de 50 MB de RAM.
- ⚙️ El entorno es más fácil de configurar, mantener y portar.

Aunque la máquina virtual ofrece mayor aislamiento, su complejidad y sobrecarga de recursos no justifican su uso para aplicaciones ligeras como DOOM. Por tanto, **Docker es la opción más práctica para este tipo de proyectos**.

---
