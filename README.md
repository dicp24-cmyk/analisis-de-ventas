# Análisis de ventas – TecnoAndes

Proyecto de análisis de datos con **Python (pandas y matplotlib)** sobre las ventas de una empresa ficticia, TecnoAndes, que vende productos de tecnología, oficina y software en 4 regiones.

El análisis responde 12 ejercicios de nivel básico a avanzado y termina con una recomendación para la gerencia comercial.

## Datos

| | |
|---|---|
| **Archivo** | `practica_analisis_datos_empresariales.xlsx` (hoja `Ventas`) |
| **Registros** | 150 transacciones |
| **Período** | enero 2025 – octubre 2026 (sin datos de noviembre y diciembre de 2025) |
| **Moneda** | USD |
| **Variables** | fecha, región, vendedor, producto, categoría, unidades, precio unitario, descuento, costo unitario, ingreso, costo total, margen y margen % |

Los datos no tienen nulos ni duplicados.

## Contenido del repositorio

- `analisis_ventas.ipynb`: notebook con todo el análisis, gráficos y conclusiones.
- `practica_analisis_datos_empresariales.xlsx`: base de datos y enunciados de los ejercicios.

## Resultados principales

| Indicador | Resultado |
|---|---|
| Ingreso total | **1.902.425 USD** |
| Margen total | **23,2 %** |
| Región con más ingreso | **Sur** (633.974 USD) |
| Producto con más unidades vendidas | **Laptop Pro** (718) |
| Vendedor con mayor margen | **Tomás Araya** (98.369 USD) |
| Categoría con mayor margen % | **Software** (36,0 %) |
| Ingreso del 3T 2026 | **383.664 USD** |
| Crecimiento ene–oct 2026 vs. 2025 | **+39,1 %** |
| Descuento promedio (solo ventas con descuento) | **17,8 %** |
| Ventas con margen negativo | **6** |

## Hallazgos

- **Crecimiento:** el ingreso de enero a octubre de 2026 es un 39 % mayor que en el mismo período de 2025. En 2025 las ventas fueron muy irregulares, y en 2026 se mantienen más altas y estables desde mayo.
- **Software es lo más rentable.** Licencia CRM y Software Contable tienen márgenes de 37 % y 35 %. Laptop Pro es el producto que más se vende, pero deja solo cerca de 15 % de margen.
- **Los descuentos altos dañan el margen.** Con descuentos de 25 % o 30 % el margen baja a cerca de 7 %, frente a más de 30 % cuando no hay descuento o es de 5 %. Las 6 ventas con pérdida tuvieron todas un 30 % de descuento.

## Recomendación

Limitar los descuentos a un máximo de **20 %** (o exigir aprobación para descuentos mayores) y reforzar la venta de **Software**, donde el margen es más alto.

## Cómo ejecutarlo

**En Google Colab**

1. Abre `analisis_ventas.ipynb` en Colab.
2. Sube `practica_analisis_datos_empresariales.xlsx` al panel de archivos.
3. Ejecuta todo con **Entorno de ejecución → Ejecutar todo**.

**En local**

```bash
pip install pandas matplotlib openpyxl jupyter
jupyter notebook analisis_ventas.ipynb
```

El Excel debe estar en la misma carpeta que el notebook.

## Herramientas

Python · pandas · matplotlib · Jupyter / Google Colab
