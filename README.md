Proyecto de Análisis de Churn para TelecomX


Descripción General
Este proyecto tiene como objetivo analizar los datos de clientes de TelecomX para identificar los factores clave que contribuyen a la 'fuga de clientes' o Churn. A través de un proceso de extracción, transformación, carga y análisis de datos, se busca comprender el comportamiento del cliente y proponer estrategias efectivas para mejorar la retención.

Fuente de Datos
Los datos provienen del archivo TelecomX_Data.json, que contiene información detallada sobre los clientes, sus servicios telefónicos e de internet, y sus cuentas.


Objetivos del Proyecto:
Identificar la tasa general de Churn en la base de clientes de TelecomX.
Explorar la relación entre variables demográficas, contractuales, de servicio y de pago con el Churn.
Generar insights accionables para la toma de decisiones estratégicas.
Proponer recomendaciones concretas para reducir la tasa de Churn.


Metodología
Extracción de Datos: Carga de los datos desde el archivo JSON.
Transformación y Normalización: Aplanamiento de las estructuras de datos anidadas (customer, phone, internet, account) en un DataFrame plano de pandas para facilitar el análisis. Creación de la columna cuenta_diaria.
Limpieza de Datos: Manejo de valores faltantes y corrección de tipos de datos, como la conversión de account.Charges.Total a numérico.
Análisis Exploratorio de Datos (EDA):
Análisis descriptivo de variables clave.
Visualización de la distribución del Churn.
Análisis de Churn por variables categóricas (tipo de contrato, género, método de pago).
Análisis de variables numéricas vs. Churn (antigüedad, cargos mensuales, total gastado).


Insights Clave
Tasa de Churn: La tasa general de Churn es del 26.54%, lo que representa un desafío significativo.
Tipo de Contrato: Los clientes con contratos mes a mes tienen la tasa de Churn más alta (42.7%), mientras que los contratos de uno y dos años muestran tasas de Churn significativamente más bajas (11.3% y 2.8% respectivamente).
Método de Pago: El cheque electrónico está asociado con la tasa de Churn más alta (45.3%), sugiriendo posibles insatisfacciones con este método o un perfil de cliente menos comprometido.
Antigüedad (Tenure): Los clientes que abandonan el servicio tienen una antigüedad promedio de 17.98 meses, considerablemente menor que los clientes retenidos (37.57 meses), indicando que el Churn es más común en las primeras etapas.
Cargos Mensuales y Totales: Los clientes que se van tienen cargos mensuales ligeramente más altos ( 74.44)yuntotalgastadosignificativamentemenor( 1531.80) en comparación con los clientes retenidos.
Género: El género no es un factor diferenciador significativo en la tasa de Churn.


Recomendaciones
Estrategias de Fidelización para Contratos Mes a Mes: Ofrecer incentivos (descuentos, mejoras de servicio, programas de lealtad) para que los clientes migren a contratos de mayor duración.
Optimización del Proceso de Pago con Cheque Electrónico: Investigar las causas de la alta tasa de Churn asociada a este método de pago y promover activamente la adopción de métodos de pago automáticos (transferencias bancarias, tarjetas de crédito) mediante beneficios o facilidades.
Programas de Retención Temprana: Implementar programas de bienvenida robustos, monitorear activamente a los clientes con baja antigüedad e implementar alertas de Churn para realizar intervenciones personalizadas.
Evaluación de Precios y Valor Percibido: Realizar un análisis de la competitividad de los precios y asegurar que los clientes perciban el valor de los servicios, especialmente aquellos con cargos mensuales más altos.


Conclusión
Al implementar estas recomendaciones basadas en los insights derivados del análisis de datos, TelecomX puede mejorar sustancialmente sus esfuerzos de retención de clientes y reducir la tasa de Churn, lo que se traducirá en una mayor lealtad del cliente y crecimiento sostenible.

