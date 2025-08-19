# Análisis de la Evasión de Clientes (Churn) en Telecom X 📉
Este proyecto es un Análisis Exploratorio de Datos (EDA) centrado en identificar los factores que influyen en la evasión de clientes (Churn) de la compañía de telecomunicaciones Telecom X. El objetivo es comprender por qué los clientes se van y ofrecer recomendaciones estratégicas basadas en datos para mejorar la retención.

🛠️ Tecnologías y Librerías
El análisis se realizó utilizando el lenguaje de programación Python y las siguientes librerías principales:

Pandas: Para la manipulación y limpieza de los datos.

NumPy: Para operaciones numéricas.

Matplotlib y Seaborn: Para la creación de visualizaciones estáticas.

Plotly: Para gráficos interactivos.

Requests: Para la extracción de los datos desde la URL.

Scikit-learn (IterativeImputer): Para el manejo avanzado de valores nulos.

🔍 Proceso de Análisis
El proyecto se estructuró en tres fases clave:

Extracción (ETL)
Se descargaron los datos en formato JSON directamente desde una URL.

Se cargaron los datos en un DataFrame de Pandas para su posterior manipulación.

Transformación (ETL)
Normalización y Limpieza: Se normalizaron las columnas anidadas y se renombraron para una mayor claridad.

Manejo de Inconsistencias: Se trataron valores nulos, strings vacíos y se convirtieron los tipos de datos a un formato adecuado (por ejemplo, binario, categórico, numérico). La imputación de los valores nulos en la columna Evasion se realizó con IterativeImputer, una técnica avanzada para evitar sesgos.

Creación de Nuevas Características: Se generó una nueva columna Factura_Diaria para un análisis más detallado.

Traducción de Columnas: Se tradujeron los nombres de las columnas a español para una mejor comprensión.

Carga y Análisis
Estadísticas Descriptivas: Se calcularon resúmenes estadísticos de las variables numéricas y categóricas.

Visualizaciones: Se crearon diversos gráficos (barras, circulares, boxplots, mapas de calor) para explorar la relación entre la evasión y otras variables.

📊 Hallazgos Clave
El análisis exploratorio reveló los siguientes factores determinantes en la evasión de clientes:

Tipo de Contrato: Los clientes con contratos mes a mes tienen una tasa de evasión significativamente más alta.

Antigüedad (Meses_Contrato): Los clientes con poca antigüedad son los más propensos a irse.

Servicio de Internet: Los clientes con servicio de Fibra Óptica presentan una evasión notablemente alta, sugiriendo problemas de calidad o soporte.

Servicios Adicionales: Los clientes que no contratan servicios adicionales como Seguridad_EnLinea o Soporte_Tecnico tienen una mayor probabilidad de evasión.

Facturación: Los clientes que evaden tienden a tener facturas mensuales y diarias más altas.

Método de Pago: El uso de cheque electrónico está fuertemente correlacionado con una mayor tasa de abandono.

📄 Conclusiones y Recomendaciones
Basado en los hallazgos, se proponen las siguientes acciones estratégicas para mitigar la pérdida de clientes:

Fomentar Contratos a Largo Plazo: Ofrecer incentivos y promociones para convertir a los clientes de contratos mensuales en contratos de un año o más.

Mejorar el Servicio de Fibra Óptica: Investigar y resolver los problemas subyacentes que afectan la experiencia de los usuarios de este servicio.

Incentivar Servicios Adicionales: Promover la contratación de paquetes que incluyan servicios de valor agregado para aumentar la retención.

Optimizar Métodos de Pago: Animar a los clientes a usar métodos de pago automáticos para reducir la fricción en el proceso de facturación.

Programa de Retención Proactivo: Crear un programa de seguimiento para clientes nuevos y aquellos con poca antigüedad para abordar sus necesidades antes de que decidan irse.
