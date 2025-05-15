# 🎮 Proyecto: Comparativa de Rendimiento - Docker 🐳 vs Máquina Virtual 🖥️ con DOOM en Windows

Este proyecto evalúa el rendimiento de un juego clásico **Chocolate DOOM** ejecutado en dos entornos distintos:  
- Contenedores **Docker**  
- Máquinas Virtuales **VirtualBox**  

ambos sobre sistemas operativos Windows. La comparativa se centra en análisis técnico, rendimiento, consumo de recursos y facilidad de mantenimiento.

---

## 📂 Estructura del Proyecto

comparativa-doom/
├── README.md
├── metricas.md
├── docker/
│ └── Dockerfile
├── vm/
│ └── instrucciones_vm.md
├── screenshots/
│ └── grafico_estructura.png
└── requirements.txt



---

## 3. Requisitos

- 💻 **Sistema Operativo Host**: Windows 10/11  
- 🧰 **Hardware**: CPU Intel i7, 16 GB RAM, SSD 512 GB  
- 🛠️ **Software Necesario**:  
  - Docker Desktop (con WSL2 activado)  
  - Oracle VirtualBox  
  - Ubuntu 20.04 (ISO)  
  - Chocolate Doom (versión Linux)  

Instala Chocolate Doom en Ubuntu con:  
```bash
sudo apt update && sudo apt install chocolate-doom
