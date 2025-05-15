# 4. Objetivos del Proyecto
⏱️ Evaluar el tiempo de arranque de Chocolate Doom

📊 Medir el consumo de RAM en ambos entornos

🔧 Analizar facilidad de implementación y mantenimiento

# 5. Comparativa Técnica

**Docker (WSL2)**
- ⏳ Tiempo de arranque: ~1.2 segundos
- 🧠 Uso de RAM: ~48 MB
- 🖥️ Interfaz gráfica: Terminal (SDL)
- 🔧 Mantenimiento: Fácil
- 📦 Portabilidad: Alta
- 🔐 Seguridad: Menor

**Máquina Virtual (VirtualBox)**
- ⏳ Tiempo de arranque: ~29 segundos
- 🧠 Uso de RAM: ~210 MB
- 🖥️ Interfaz gráfica: Ventana completa (X11/SDL)
- 🔧 Mantenimiento: Complejo
- 📦 Portabilidad: Media
- 🔐 Seguridad: Alta

# 6. Métricas Técnicas - Resultados de 3 Días

**Resultados:**
- **Día 1**
  - Docker: Tiempo (s): 1.2
  - Docker: RAM (MB): 48
  - VM: Tiempo (s): 28
  - VM: RAM (MB): 210

- **Día 2**
  - Docker: Tiempo (s): 1.1
  - Docker: RAM (MB): 50
  - VM: Tiempo (s): 30
  - VM: RAM (MB): 205

- **Día 3**
  - Docker: Tiempo (s): 1.3
  - Docker: RAM (MB): 47
  - VM: Tiempo (s): 29
  - VM: RAM (MB): 215

  # 7. Entornos de Prueba

**Docker en Windows (WSL2)**
- 🖥️ SO Invitado: Ubuntu 20.04 (WSL2)
- ⚙️ Recursos Asignados: 2 CPU, 4 GB RAM
- 💾 Disco utilizado: 1 GB imagen Docker
- 🖥️ Interfaz de ejecución: Terminal (SDL modo texto)

**Máquina Virtual (VirtualBox)**
- 🖥️ SO Invitado: Ubuntu 20.04
- ⚙️ Recursos Asignados: 2 CPU, 4 GB RAM
- 💾 Disco utilizado: 10 GB disco virtual
- 🖥️ Interfaz de ejecución: Ventana gráfica completa

# 8. Herramientas Utilizadas
- Docker Desktop (WSL2)
- Oracle VirtualBox
- Ubuntu 20.04 LTS
- Chocolate Doom (sudo apt install chocolate-doom)
- htop y time para medición de uso y rendimiento

# 9. Gráfico Comparativo de Estructura
```mermaid
graph TD
    A[🪟 Windows Host] --> B[🐳 Docker + WSL2 - Doom]
    A --> C[🖥️ VirtualBox VM - Ubuntu - Doom]
    B --> D[🎮 Chocolate Doom (SDL en terminal)]
    C --> E[🎮 Chocolate Doom (interfaz X11)]

    
---

### 10. Observaciones Técnicas

```markdown
# 10. Observaciones Técnicas
- Docker inicia Doom en ~1 segundo gracias a su arquitectura ligera. 🚀
- La VM demora ~30 segundos en iniciar debido a la carga completa del sistema operativo. 🐢
- El uso de RAM en Docker fue significativamente menor. 📉
- Mantenimiento del entorno Docker es más sencillo (limpieza de contenedores, actualización de imágenes). 🔄
- VM ofrece mayor aislamiento, pero a costa de rendimiento y complejidad. 🔐
