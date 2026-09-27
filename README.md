Plataforma Académica Básica
Integrantes
Hermes Jose Cantillo Perez
Yesid Alexander Alonso Villamarin
---
Descripción del proyecto
La Plataforma Académica Básica es un proyecto orientado al procesamiento, visualización y análisis de información generada por los vehículos del Sistema Integrado de Transporte Público (SITP).
Actualmente, los vehículos del SITP generan aproximadamente cada 20 segundos una trama de datos en formato tipo JSON, que contiene información relevante para el seguimiento y análisis de las condiciones operativas del vehículo.
Entre los datos registrados se encuentran:
ID del vehículo.
Fecha y hora del registro.
Geolocalización.
Nivel de batería, en el caso de vehículos eléctricos.
Pastilla de freno con menor nivel de desgaste.
Velocidad.
Temperatura del motor.
Temperatura de la batería.
Temperatura de la CPU.
Odómetro.
Debido al volumen y frecuencia con los que se generan estos datos, surge la necesidad de contar con una herramienta que permita visualizar, relacionar y analizar la información de manera rápida y organizada.
La plataforma busca proporcionar una representación gráfica de los datos, permitiendo realizar un análisis que vaya de lo macro a lo micro. De esta manera, el usuario podrá obtener inicialmente una visión general del comportamiento de la flota y posteriormente profundizar en vehículos, variables o registros específicos.
Además, el sistema contempla la identificación de datos atípicos, con el propósito de facilitar la detección de comportamientos que se alejen de los patrones esperados y que puedan requerir una revisión posterior.
---
Objetivo general
Desarrollar una plataforma que permita visualizar, relacionar y analizar de manera eficiente los datos generados por los vehículos del SITP, facilitando la identificación de patrones y datos atípicos mediante herramientas de visualización y análisis.
---
Objetivos específicos
Procesar las tramas de datos generadas por los vehículos del SITP en formato tipo JSON.
Organizar y almacenar la información obtenida de las diferentes variables de los vehículos.
Implementar mecanismos de visualización que permitan analizar la información desde una perspectiva general hasta un nivel detallado.
Relacionar diferentes variables para facilitar el análisis del comportamiento de los vehículos.
Identificar datos atípicos que puedan representar comportamientos fuera de los patrones esperados.
Presentar la información de manera clara para facilitar su interpretación y análisis.
---
Variables analizadas
Variable	Descripción
ID del vehículo	Identificador único del vehículo
Fecha y hora	Momento en que se genera el registro
Geolocalización	Ubicación del vehículo
Nivel de batería	Porcentaje o nivel disponible en vehículos eléctricos
Desgaste de freno	Nivel de desgaste de la pastilla de freno con menor rendimiento
Velocidad	Velocidad registrada por el vehículo
Temperatura del motor	Temperatura registrada en el motor
Temperatura de batería	Temperatura de la batería del vehículo
Temperatura de CPU	Temperatura registrada en la unidad de procesamiento
Odómetro	Distancia acumulada recorrida por el vehículo
---
Funcionalidades principales
Recepción y procesamiento de datos: procesamiento de las tramas generadas por los vehículos.
Visualización de información: representación gráfica de las variables registradas.
Análisis de datos: consulta y comparación de diferentes variables.
Análisis geográfico: visualización de la ubicación de los vehículos.
Análisis de tendencias: identificación de comportamientos en las variables registradas.
Detección de datos atípicos: identificación de valores que presentan comportamientos fuera de los patrones establecidos.
Análisis de lo macro a lo micro: visualización general de la flota y posterior exploración detallada de vehículos y variables específicas.
---
Flujo general del sistema
```text
Tramas de datos de vehículos SITP
              │
              ▼
      Recepción de datos
              │
              ▼
       Procesamiento JSON
              │
              ▼
      Organización de datos
              │
              ▼
       Almacenamiento
              │
              ▼
     Análisis y correlación
              │
        ┌─────┴─────┐
        ▼           ▼
 Visualización   Detección
    gráfica     de atípicos
        │           │
        └─────┬─────┘
              ▼
       Análisis final
```
---
Enfoque de visualización
La plataforma plantea un modelo de análisis de lo macro a lo micro.
Nivel macro
Permite obtener una visión general de la flota, identificando tendencias, distribución de vehículos, comportamiento general de las variables y posibles situaciones anómalas.
Nivel intermedio
Permite analizar grupos de vehículos, zonas geográficas, periodos de tiempo o determinadas variables.
Nivel micro
Permite profundizar en un vehículo específico y consultar detalladamente sus registros, variables, comportamiento histórico y posibles datos atípicos.
---
Detección de datos atípicos
Uno de los componentes principales del proyecto es la identificación de datos atípicos, entendidos como valores que presentan un comportamiento significativamente diferente respecto al patrón esperado.
El análisis podrá considerar variables como:
Velocidad.
Temperatura del motor.
Temperatura de la batería.
Temperatura de la CPU.
Nivel de batería.
Desgaste de frenos.
Ubicación.
Odómetro.
La detección de estos comportamientos permitirá generar información útil para posteriores procesos de análisis y toma de decisiones operativas.
---
Tecnologías
Las tecnologías definitivas dependerán de la implementación del proyecto. Entre las herramientas contempladas se encuentran:
Python
JSON
Bases de datos
Git
GitHub
Herramientas de visualización y análisis de datos.
---
Estructura del proyecto
```text
Plataforma-Academica-Basica/
│
├── README.md
├── datos/
│   └── tramas.json
│
├── src/
│   ├── procesamiento/
│   ├── analisis/
│   └── visualizacion/
│
├── pruebas/
│
└── documentacion/
```
> La estructura anterior puede modificarse de acuerdo con la implementación definitiva del proyecto.
---
Estado del proyecto
En desarrollo.
Actualmente, el proyecto se encuentra orientado al diseño e implementación de una solución para el procesamiento, análisis y visualización de las tramas de datos generadas por los vehículos del SITP.
---
Propósito académico
Este proyecto se desarrolla con fines académicos y tiene como propósito aplicar conocimientos relacionados con desarrollo de software, procesamiento de datos, almacenamiento de información, análisis de datos, visualización y detección de comportamientos atípicos.
La solución busca integrar estos conceptos en una aplicación que permita transformar grandes cantidades de datos provenientes de los vehículos en información organizada y útil para su análisis.
---
Autores
Hermes Jose Cantillo Perez  
Yesid Alexander Alonso Villamarin
Proyecto académico — 2026
