# Proyecto 10: Toma de Decisiones Basada en Datos
> **Priorización de Hipótesis y Análisis de Test A/B para Maximización de Ingresos**

## 📋 Descripción
Este proyecto consistió en priorizar hipótesis de negocio utilizando frameworks estratégicos y validar el impacto de los cambios mediante un Test A/B riguroso, analizando conversiones e ingresos.

## 🎯 Fase 1: Priorización (ICE vs RICE)
Se evaluaron 9 hipótesis para determinar el orden de ejecución.

| Hipótesis | ICE Rank | RICE Rank | Hallazgo Clave |
| :--- | :---: | :---: | :--- |
| **#8** (Descuentos) | 1º | 5º | Gran impacto, pero alcance (Reach) limitado. |
| **#7** (Suscripción) | 3º | 1º | El alto **alcance** compensa su menor impacto individual. |



---

## 🧪 Fase 2: Análisis del Test A/B
Se comparó el comportamiento de los grupos **A (Control)** y **B (Prueba)** durante agosto de 2019.

### 📈 Resultados en Datos Brutos
* **Ingresos:** El grupo B superó significativamente al A, especialmente a partir del 19 de agosto.
* **Conversión:** Grupo B (**3.10%**) vs Grupo A (**2.68%**).

### 🧹 Limpieza de Anomalías (Percentiles 95 y 99)
Para evitar sesgos por "compras atípicas", se filtraron los datos:
* **Pedidos por usuario:** El 99% de los usuarios hace 2 pedidos o menos.
* **Ingreso por pedido:** Se eliminaron pedidos superiores a **$830.3** (incluyendo un pedido anómalo de $20,000).



### 📊 Significancia Estadística (Datos Filtrados)
Tras el filtrado, los resultados confirmaron la tendencia:
1. **Conversión:** El Grupo B mantuvo una ventaja real y estadísticamente significativa ($p < 0.05$).
2. **Ticket Promedio:** Aunque el Grupo B registró un promedio mayor ($145 vs $115), la diferencia no fue estadísticamente significativa tras el filtrado ($p = 0.404$).

## 🏁 Decisión Final
**Conclusión: DETENER LA PRUEBA Y DECLARAR GANADOR AL GRUPO B.**
La tasa de conversión del Grupo B es superior y estable, lo que garantiza un incremento en los ingresos totales del negocio a largo plazo.

---
🔗 [**Ver Notebook Completo**](https://github.com/LuisPeza/Proyecto_10/blob/main/Proyecto_10_Tomar%20decisiones%20basada%20en%20datos%20Tienda%20online.ipynb)
