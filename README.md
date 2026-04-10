# WinGameOptimizer

Herramienta de optimizacion de Windows para gaming. Detecta tu hardware y aplica ajustes de rendimiento automaticamente.

## Descarga

Descarga la ultima version desde [**Releases**](https://github.com/LetalDark/WinGameOptimizer/releases):

- **WinGameOptimizer-GUI.exe** — Interfaz grafica (recomendado)
- **WinGameOptimizer-CLI.exe** — Version consola

> **Ejecutar como Administrador** (clic derecho > Ejecutar como administrador)

No necesita instalar .NET — los exe son autocontenidos.

## Que hace

### Deteccion de hardware
- CPU (nucleos, boost, cache L3)
- GPU (VRAM, PCIe, ReBAR, driver) — via GPU-Z
- RAM (modulos, velocidad, CAS latency, XMP, canal dual/single) — via CPU-Z
- Monitor (resolucion, Hz, HDR, GSync/FreeSync)
- Almacenamiento (SSD/HDD, espacio libre)
- Red (adaptador, velocidad)
- Sistema (version Windows, Game Mode, HAGS)

### Optimizaciones (13 ajustes)
| Optimizacion | Efecto |
|---|---|
| VBS / HVCI | +2-10% FPS — reduce seguridad de virtualizacion |
| Game DVR / Game Bar | Desactiva captura en segundo plano |
| Timer Resolution (Win11) | Mejor frame pacing |
| MMCSS Gaming Priority | Prioridad CPU/GPU/red para juegos |
| HAGS | GPU Scheduling con deteccion inteligente |
| BypassIO (DirectStorage) | Necesario para DirectStorage en NVMe |
| MPO | Soluciona stuttering y flickering |
| Plan de energia | Maximo rendimiento |
| Aceleracion de raton | Precision consistente + test polling rate |
| Shader Cache AMD | Menos micro-cortes (RX 5000-9000) |
| Shader Cache NVIDIA | Reduce tiempos de compilacion de shaders |
| Pagefile | Archivo de paginacion optimizado para SSD |
| Control Flow Guard (CFG) | Reduce tiempos de shaders en juegos DX12 |

### Diagnosticos
- Uso de RAM y top procesos
- Antivirus activos
- Procesos pesados en background
- Overlays (Steam, GeForce, Discord)
- Driver GPU desactualizado
- Espacio en disco
- Apps de inicio (con opcion de desactivar)

### Otras funciones
- Modo automatico (aplica todo de una vez)
- Advertencias si XMP o ReBAR estan desactivados
- Backup automatico del registro antes de cada cambio
- Boton Revertir en cada optimizacion
- Auto-actualizacion desde GitHub Releases

## Requisitos

- Windows 10/11 (64-bit)
- Ejecutar como Administrador

## Licencia

Uso personal.
