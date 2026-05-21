# Análisis de Retención y Comportamiento de Clientes (E-commerce) 🛒📈

Este proyecto simula un entorno empresarial real donde se extraen datos transaccionales directamente desde un servidor de producción para analizar el comportamiento, fidelidad y ticket medio de los clientes de un e-commerce tecnológico.

## 🛠️ Tecnologías y Arquitectura del Pipeline
El flujo de trabajo técnico se diseñó imitando las prácticas de la industria:
1. **Almacenamiento (Base de Datos Relacional):** Diseño y modelado de tablas (`usuarios` y `pedidos`) en **MySQL**, definiendo claves primarias, foráneas (`FOREIGN KEY`) y tipos de datos óptimos.
2. **Extracción y Conexión:** Uso de `mysql-connector-python` para comunicar el servidor local de bases de datos con el entorno analítico.
3. **Procesamiento y Fusión de Datos:** Manipulación y combinación de dataframes mediante **Pandas** (`pd.merge`, `groupby`, `mean`, `count`).
4. **Visualización Avanzada:** Creación de gráficos profesionales y estilizados utilizando **Seaborn** y **Matplotlib**.

## 📊 Métricas de Negocio e Insights Clave

* **Alta Tasa de Fidelización:** El **80% de los clientes** registrados volvieron a comprar en la plataforma al menos una segunda vez. El cliente más frecuente es Carlos Mendoza con 3 pedidos.
* **Relación Inversa (Frecuencia vs. Gasto):** Se identificó que el cliente con mayor volumen de pedidos (Carlos Mendoza) registra un ticket medio bajo ($265.00), mientras que el cliente con menor frecuencia (Lucas Rossi, 1 pedido) posee el ticket medio más alto del negocio ($950.00). 
  * *Estrategia propuesta:* Campañas de up-selling para subir el ticket medio de Carlos y acciones de remarketing para reactivar la frecuencia de Lucas.
* **Categorías Core:** Los productos de la categoría **Laptops** lideran el volumen total de ingresos facturados, seguidos muy de cerca por **Smartphones**.

## 📂 Estructura de este Repositorio
* `Analisis_retencion_clientes.ipynb`: Notebook principal con todo el código documentado, el control de warnings y las visualizaciones limpias.
