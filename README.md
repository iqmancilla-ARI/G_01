# Sprint 01 — Limpieza y Preparación de Datos de Clientes

> **TripleTen Data Science Bootcamp · Sprint 1 · Proyecto Integrador**

## Descripción

Proyecto de introducción al procesamiento de datos con Python, enfocado en la limpieza y estandarización de registros de clientes para el equipo de análisis de **Store 1**. El objetivo es preparar un dataset de usuarios para futuros análisis de negocio: identificación de clientes leales, análisis de ingresos por categoría y segmentación para campañas de marketing.

---

## Objetivos del Proyecto

- Limpiar y normalizar nombres de usuario (espacios, separadores, capitalización)
- Validar y convertir tipos de datos (edades como enteros, manejo de errores)
- Ordenar registros por ID de cliente
- Calcular gasto total por categorías de compra
- Generar cadenas de resumen para reportes ejecutivos
- Construir un pipeline completo de limpieza sobre múltiples registros

---

## Estructura del Notebook

| Paso | Descripción | Técnicas aplicadas |
|------|-------------|-------------------|
| 1 | Limpieza de nombres: espacios y separadores | `strip()`, `replace()` |
| 2 | Separación de nombre y apellido | `split()` |
| 3 | Conversión de tipo de dato en edad | `int()` |
| 4 | Manejo de edades inválidas | `try / except` |
| 5 | Ordenamiento de registros por ID | `list.sort()` |
| 6 | Cálculo de gasto total por categoría | Indexación de listas |
| 7 | Generación de resumen por cliente | `str.format()` |
| 8 | Conteo de registros registrados | `len()`, `str.format()` |
| 9 | Pipeline completo de limpieza sobre múltiples usuarios | Integración de todos los pasos anteriores |

---

## Stack Técnico

- **Python 3**
- **Jupyter Notebook**
- Librerías estándar: sin dependencias externas

---

## Estructura de Datos

Cada registro de usuario tiene el siguiente formato:

```python
[id, nombre, edad, [categorías_favoritas], [gastos_por_categoría]]

# Ejemplo:
['32415', ' mike_reed ', 32.0, ['ELECTRÓNICA', 'DEPORTE', 'LIBROS'], [894, 213, 173]]
```

---

## Resultados

El notebook produce una lista `usuarios_limpio` con registros estandarizados:
- Nombres limpios y separados en `[nombre, apellido]`
- Edades como enteros válidos
- Registros ordenados por ID ascendente
- Gasto total calculado por cliente

---

## Aprendizajes Clave

- Uso de métodos de cadenas para limpieza de texto (`strip`, `replace`, `split`, `format`)
- Control de errores con `try/except` para datos no válidos
- Manipulación de listas anidadas (estructuras tipo registro)
- Buenas prácticas: se identifica la oportunidad de refactorizar bloques repetidos en un bucle `for` para mejorar mantenibilidad

---

## Autor

**J. Daniel Mancilla Malvaez**  
Ingeniero Químico | Industrial Operations & Data Science  
[LinkedIn](https://linkedin.com/in/pmomancilla) · [GitHub](https://github.com/iqmancilla-ARI)
