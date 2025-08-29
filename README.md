
# 📊 Dashboard Financiero en Power BI

## 📌 Executive Summary

Este proyecto presenta un **Dashboard Financiero en Power BI** diseñado a partir de un plan contable estructurado (NIVEL 1–5).  
El tablero integra **análisis horizontal, vertical e indicadores financieros clave** (liquidez, endeudamiento y rentabilidad) para evaluar la salud financiera de la empresa.

### 🔑 Principales hallazgos
- **Estructura patrimonial sólida**: más del 90% de los activos financiados con patrimonio.  
- **Liquidez destacada**: Liquidez General = 3.09 y Prueba Ácida = 3.21 → excelente capacidad de pago.  
- **Endeudamiento bajo**: relación Pasivo/Patrimonio de 0.10 → autonomía financiera.  
- **Rentabilidad sobresaliente**: Margen Neto 28,5%, ROA 42% y ROE > 1000% (influenciado por bajo capital social).  
- **Riesgos identificados**: caída de ingresos en 2019 (-15,6%) y concentración de activos en cuentas por cobrar.

### 📌 Recomendaciones
1. **Ampliar el modelo** incorporando estados de flujo de efectivo para un análisis de solvencia más robusto.  
2. **Conectar a una fuente dinámica** (Excel, SQL, API) para que el dashboard se actualice automáticamente.  
3. **Enriquecer el storytelling visual** agregando narrativas automáticas en DAX e indicadores de alerta.  
4. **Escalar el modelo** aplicando un enfoque de *star schema* con `FactTransacciones` y dimensiones (`DimCuenta`, `DimCalendario`).  

---


Este proyecto muestra un **análisis integral financiero y contable** de una empresa ficticia en el periodo 2017–2019.  
Se incluyen métricas de **liquidez, endeudamiento, rentabilidad y estructura patrimonial**, aplicando técnicas de análisis horizontal y vertical.  

El objetivo es demostrar cómo un **plan contable normalizado** puede convertirse en un tablero gerencial para la toma de decisiones.  

---

## 🖼️ Vistas del Dashboard

### 1. Resumen Patrimonial
![Pantallazo](img/img1.png)  
**Interpretación:**  
- Activos totales: $13,24 millones.  
- Pasivos: $1,28 millones (≈10% del activo).  
- Patrimonio: $11,96 millones (alta independencia financiera).  
📌 **Conclusión ampliada:**  
La empresa mantiene una estructura patrimonial **muy sólida**, con activos financiados en más de un 90% por patrimonio y apenas un 10% por pasivos. Esto refleja independencia financiera, bajo riesgo de solvencia y capacidad de resistir crisis externas. Sin embargo, esta baja deuda también implica que la empresa podría estar desaprovechando la oportunidad de apalancarse con financiamiento barato para acelerar su crecimiento.

---

### 2. Resumen Operativo
![Pantallazo](img/img2.png)  
**Interpretación:**  
- Ingresos: $19,71 millones.  
- Costos: $2,04 millones.  
- Gastos: $5,53 millones.  
- Resultado operativo: $17,67 millones.  
📌 **Conclusión ampliada:**  
La empresa presenta un **resultado operativo positivo y robusto**, con costos relativamente bajos frente a ingresos. Sin embargo, se observa una caída de ingresos en 2019 (-15,6%), lo que indica que, a pesar de ser rentable, la organización debe analizar causas (ejemplo: caída de demanda, aumento de competencia, cambios en precios) para asegurar sostenibilidad futura.

---

### 3. Análisis Horizontal
![Pantallazo](img/img3.png)  
**Interpretación:**  
- Crecimiento fuerte del activo no corriente (+197% en 2018).  
- Caída de ingresos (-15,6% en 2019).  
📌 **Conclusión ampliada:**  
El crecimiento del activo no corriente en 2018 (+197%) muestra una fuerte apuesta por inversión a largo plazo (posiblemente en activos fijos o mejoras de infraestructura). Esto es positivo, pero debe contrastarse con la generación de ingresos para asegurar que la inversión se traduzca en crecimiento sostenible. La caída de ingresos en 2019 es una alerta temprana que debe monitorearse.

---

### 4. Análisis Vertical
![Pantallazo](img/img4.png)  
**Interpretación:**  
- Activos concentrados en créditos por cobrar.  
- Pasivos concentrados en deudas comerciales.  
- Patrimonio explicado por resultados acumulados.  
📌 **Conclusión ampliada:**  
La concentración en **cuentas por cobrar** dentro del activo refleja una política de crédito agresiva o dependencia de pocos clientes. Esto puede ser riesgoso si la cobranza no es eficiente. En el pasivo, el peso de las deudas comerciales indica que las obligaciones son principalmente operativas y no financieras. El patrimonio está altamente explicado por resultados acumulados, lo cual es positivo pero también resalta la importancia de seguir generando utilidades.

---

### 5. Árbol de Partidas Contables
![Pantallazo](img/img5.png)  
**Interpretación:**  
- Se observa la jerarquía del plan contable desde Patrimonio → Capital Social → Resultados.  
📌 **Conclusión ampliada:**  
El árbol jerárquico permite **navegar desde el patrimonio hacia el capital social y resultados**, lo que facilita transparencia y trazabilidad contable. Este drill-down es valioso para auditores o analistas, ya que permite conectar el detalle de las transacciones con los estados financieros consolidados.

---

### 6. Análisis de Liquidez
![Pantallazo](img/img6.png)  
**Interpretación:**  
- Liquidez general: 3.09.  
- Prueba ácida: 3.21.  
- Rotación de cuentas por cobrar: 64 veces/año.  
📌 **Conclusión ampliada:**  
Los indicadores de liquidez son excelentes (Liquidez general 3.09 y Prueba ácida 3.21). Esto significa que la empresa podría cubrir tres veces sus obligaciones de corto plazo con activos líquidos. Además, la alta rotación de cuentas por cobrar (64 veces al año) indica que la empresa cobra muy rápido a sus clientes. Esto genera una **posición de caja muy cómoda**, aunque también podría reflejar que la empresa ofrece poco crédito, limitando potencial de ventas.

---

### 7. Análisis de Endeudamiento
![Pantallazo](img/img7.png)  
**Interpretación:**  
- Endeudamiento total: 0.10.  
- La mayor parte es pasivo corriente.  
📌 **Conclusión ampliada:**  
El endeudamiento total es apenas de 0.10, con la mayor parte concentrada en pasivos de corto plazo. Esto significa que la empresa tiene **margen para asumir deuda de largo plazo** y financiar proyectos de expansión sin comprometer su estabilidad. Sin embargo, depender demasiado del patrimonio puede significar menor rendimiento financiero por falta de apalancamiento.

---

### 8. Análisis de Rentabilidad
![Pantallazo](img/img8.png)  
**Interpretación:**  
- Margen bruto: 89,5%.  
- Margen neto: 28,5%.  
- ROA: 42%.  
- ROE: 1507%.  
📌 **Conclusión ampliada:**  
La rentabilidad es sobresaliente: margen bruto 89,5%, margen neto 28,5%, ROA 42% y ROE superior al 1000%. Esto último se explica por un capital social muy bajo en comparación con las utilidades, lo que dispara el ROE. Aunque estos indicadores son positivos, es importante analizar su sostenibilidad: un ROE tan alto podría no ser replicable en el largo plazo si no se reinvierte capital o no se controla la caída de ingresos observada en 2019.

---

## 📖 Diccionario de Datos

| Campo | Tipo | Descripción | Ejemplo |
|-------|------|-------------|---------|
| **CUENTA** | Texto | Código contable según PCGE/empresa. | 6030130001 |
| **NOMBRE DE LA CUENTA** | Texto | Nombre de la cuenta contable. | MANTENIMIENTO DE TRACTORES |
| **Fecha** | Fecha | Fecha contable de la transacción. | 01/05/2017 |
| **Monto** | Decimal | Valor monetario de la transacción. | 1250.50 |
| **CUENTA T** | Texto | Cuenta T o agrupadora. | 6030113001 |
| **NIVEL 1** | Texto | Clase principal (Activo, Pasivo, Patrimonio, Ingresos, Gastos, Costos). | GASTOS |
| **NIVEL 2** | Texto | Subclase (ej. Gastos de Operación). | GASTOS DE OPERACIÓN |
| **NIVEL 3** | Texto | Agrupación detallada. | GASTOS ADMINISTRATIVOS |
| **NIVEL 4** | Texto | Subagrupación específica. | MANTENIMIENTOS CORRECTIVOS |
| **NIVEL 5** | Texto | Detalle más específico. | MANTENIMIENTO DE FUMIGADORA |
| **Orden** | Entero | Control de orden en reportes. | 5 |

---

## 📚 Explicación de Indicadores Financieros

### 🔹 Liquidez
Miden la capacidad de la empresa para cumplir con sus obligaciones de corto plazo.

- **Liquidez General = Activo Corriente / Pasivo Corriente**  
  - Indica cuántas veces los activos líquidos cubren las deudas de corto plazo.  
  - Valor recomendado: **≥ 1.5**.

- **Prueba Ácida = (Activo Corriente – Inventarios) / Pasivo Corriente**  
  - Similar a la liquidez general, pero elimina inventarios por ser menos líquidos.  
  - Valor recomendado: **≥ 1.0**.

- **Días de Cuentas por Cobrar (DSO)**  
  _Medida implementada en el modelo (usa 360 días por convención)_  
  ```DAX
  Dias Cuentas por Cobrar := 
  VAR CXC =
      CALCULATE( [Total Activo], KEEPFILTERS( DATA[NIVEL 4] = "SERVICIOS POR COBRAR" ) )
  VAR ING_OP =
      CALCULATE( [Total Ingresos], FILTER( DATA, DATA[NIVEL 2] = "INGRESOS OPERATIVOS" ) )
  RETURN DIVIDE( CXC, ING_OP ) * 360
  ```
  - **Interpretación:** días promedio que tarda la empresa en cobrar sus ventas. Más bajo = mejor gestión de cobranzas.
  - **Equivalente en “veces por año” (rotación):** `Rotación CxC = ING_OP / CXC`.

- **Días de Inventario (DIO)**  
  _Medida implementada en el modelo (usa 360 días por convención)_  
  ```DAX
  Dias de Inventario :=
  VAR Inventario =
      CALCULATE( [Total Activo], FILTER( DATA, DATA[NIVEL 3] = "BIENES DE CAMBIO O REALIZABLE" ) )
  VAR Costo := [Total Costos]
  RETURN DIVIDE( Inventario, Costo ) * 360
  ```
  - **Interpretación:** días promedio que los bienes permanecen en inventario antes de venderse.  
  - **Más bajo es mejor** (menos inmovilización de capital).  
  - 🔎 **Nota:** si en tu modelo los costos se almacenan con signo negativo, **no multipliques por -1**; en su lugar normaliza `[Total Costos]` para que sea **positivo** en reporting.

---

### 🔹 Endeudamiento
Evalúan cuánto de los activos se financian con deuda y la capacidad para cubrir pasivos.

- **Endeudamiento Patrimonial = Pasivo Total / Patrimonio**  
  - Cuánto debe la empresa por cada sol invertido por los accionistas.

- **Endeudamiento del Activo = Pasivo Total / Activo Total**  
  - Porcentaje del activo financiado con deuda. Valores bajos (< 0.4) indican autonomía financiera.

- **Corto vs Largo Plazo**  
  - Útil para evaluar presión de liquidez si hay alta concentración en corto plazo.

---

### 🔹 Rentabilidad
Miden la eficiencia para generar utilidades.

- **Margen Bruto = (Ingresos – Costos) / Ingresos** – Eficiencia de las operaciones básicas.  
- **Margen Neto = Resultado Neto / Ingresos** – Utilidad final por sol vendido.  
- **ROA = Resultado Neto / Activo Total** – Uso eficiente de activos.  
- **ROE = Resultado Neto / Patrimonio** – Rentabilidad para los accionistas.  

> Consejo: compara con **benchmarks del sector** para dar contexto (p. ej., ROE empresa vs ROE sector).

---

## 🔎 Conclusiones Generales
1. La empresa presenta **alta solidez patrimonial** y bajo endeudamiento.  
2. Los **ingresos muestran caída en 2019**, a vigilar.  
3. Liquidez y rentabilidad son **sobresalientes**.  
4. La **concentración en cuentas por cobrar** puede ser un riesgo de liquidez futura.  
5. Se recomienda explorar **uso moderado de deuda** para expansión.  

---

✍️ **Autor:** [Tu Nombre]  
📌 Proyecto académico/portafolio en **Power BI, Contabilidad y Análisis Financiero**.  

#### ✅ Medidas de Rentabilidad (según este modelo)

> **Nota:** En este modelo, el *Resultado del Periodo* se obtiene filtrando el **Patrimonio** por `NIVEL 5 = "RESULTADOS DE LA GESTION"`.  
> Si en tu versión futura defines una medida específica `[Resultado Neto]`, puedes reemplazarla en estas fórmulas para mayor claridad.

```DAX
Ingresos Operativos :=
CALCULATE( [Total Ingresos], KEEPFILTERS( DATA[NIVEL 2] = "INGRESOS OPERATIVOS" ) )

Margen Bruto % :=
VAR IngresosOper = [Ingresos Operativos]
VAR Costos = [Total Costos]
RETURN DIVIDE( IngresosOper - Costos, IngresosOper )

Margen de Utilidad Neta % :=
VAR ResultadoNeto =
    CALCULATE( [Total Patrimonio], KEEPFILTERS( DATA[NIVEL 5] = "RESULTADOS DE LA GESTION" ) )
RETURN DIVIDE( ResultadoNeto, [Ingresos Operativos] )

Rendimiento del Capital (ROE) % :=
VAR ResultadoNeto =
    CALCULATE( [Total Patrimonio], KEEPFILTERS( DATA[NIVEL 5] = "RESULTADOS DE LA GESTION" ) )
VAR CapitalSocial =
    CALCULATE( [Total Patrimonio], KEEPFILTERS( DATA[NIVEL 4] = "CAPITAL SOCIAL" ) )
RETURN DIVIDE( ResultadoNeto, CapitalSocial )

Rendimiento del Activo (ROA) % :=
VAR ResultadoNeto =
    CALCULATE( [Total Patrimonio], KEEPFILTERS( DATA[NIVEL 5] = "RESULTADOS DE LA GESTION" ) )
RETURN DIVIDE( ResultadoNeto, [Total Activo] )
```

**Interpretaciones rápidas**  
- **Margen Bruto %**: rentabilidad de la operación antes de gastos; ↑ mejor eficiencia en costos.  
- **Margen de Utilidad Neta %**: utilidad final por cada sol vendido; útil para comparar periodos y peers.  
- **ROE %** (*Rendimiento del Capital*): retorno para accionistas vs capital social; valores extremos pueden indicar capital bajo o efectos no recurrentes.  
- **ROA %** (*Rendimiento del Activo*): eficiencia del uso de activos para generar utilidades.
```

**Buenas prácticas**  
- Para ROE/ROA, considera utilizar **promedio de saldos** (Activo/Patrimonio promedio del periodo) si haces análisis mensual/trimestral.
- Normaliza signos en medidas base: Ingresos (+), Costos/Gastos (+ para reporting o – si tu estándar lo requiere, pero consistente).
```
#### ✅ Medidas de Endeudamiento (según este modelo)

```DAX
Endeudamiento Patrimonial :=
DIVIDE( [Total Pasivo], [Total Patrimonio] )

Endeudamiento del Activo :=
DIVIDE( [Total Pasivo], [Total Activo] )

Endeudamiento a Corto Plazo :=
CALCULATE( [Total Pasivo], KEEPFILTERS( DATA[NIVEL 2] = "PASIVO CORRIENTE" ) )
    / [Total Patrimonio]

Endeudamiento a Largo Plazo :=
CALCULATE( [Total Pasivo], KEEPFILTERS( DATA[NIVEL 2] = "PASIVO NO CORRIENTE" ) )
    / [Total Patrimonio]
```

**Interpretaciones rápidas**  
- **Endeudamiento Patrimonial**: cuánto debe la empresa por cada sol de patrimonio.  
- **Endeudamiento del Activo**: proporción del activo financiada con deuda.  
- **Endeudamiento a Corto Plazo**: mide la presión de obligaciones inmediatas sobre el patrimonio.  
- **Endeudamiento a Largo Plazo**: mide el nivel de deuda de largo plazo frente al patrimonio.  

**Buenas prácticas**  
- Analizar la **estructura de vencimientos** (corto vs largo plazo) para evaluar riesgo de liquidez vs solvencia.  
- Un nivel bajo de endeudamiento otorga autonomía financiera, pero también puede significar desaprovechar apalancamiento estratégico para crecer.
