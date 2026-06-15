# AgentesInteligentes

# Coordinación Inteligente de Cruces Semafóricos
Simulación de un corredor urbano real en San Pedro Garza García, N.L.,
con agentes semafóricos coordinados mediante Q-Learning para optimizar
el flujo vehicular.
---
## Caso de Estudio
Corredor: **JDLV/FGR → Ahuehuetes/Nogales → Luis Elizondo → Primavera**  
Longitud total: ~955 m | 4 intersecciones | 9 orígenes de demanda
---
## Métodos Implementados
| Escenario | Descripción |
|---|---|
| Sin coordinación | Semáforos con fases desalineadas e independientes |
| Coordinación manual | Offsets empíricos con ciclo común a 40 km/h |
| Q-Learning SMA | Agentes aprenden offsets óptimos por refuerzo |
---
## Resultados Principales
| Escenario | Vehículos completados | Paradas/veh | Tiempo promedio |
|---|---|---|---|
| Sin coordinación | 36 | 1.94 | 20.1 s |
| Coordinación manual | 40 | 1.62 | 18.0 s |
| **Q-Learning SMA** | **46** | **1.50** | 19.5 s |
---
## Cómo ejecutar
1. Abrir [`semáforosE6.ipynb`](https://drive.google.com/file/d/1eqYV6gfEJalFHOFQgJwgVVeqZmoPnuQy/view?usp=sharing ) en Google Colab
2. Ejecutar todas las celdas en orden (`Runtime > Run all`)
3. La simulación ya se encuentra ejecutada
> **Dependencia externa:** `agentpy` — se instala automáticamente en la primera celda.
---
## Tecnologías
- Python 3 · NumPy · Matplotlib · AgentPy
- Coordenadas GPS reales convertidas a sistema métrico local
- Curvas de Bézier para geometría vial
- Q-Learning con ε-greedy y early stopping
---
