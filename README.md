### ¿Cuándo un cliente empieza a valer la inversión? Un viaje por los datos de Showz

#### Objetivo del proyecto
Analizar el comportamiento de los usuarios y los datos históricos de ventas, visitas y marketing para:

- Identificar fuentes de adquisición de clientes más rentables

- Calcular métricas clave como CAC, LTV y ROMI

- Determinar el momento en que los ingresos compensan el costo de adquisición

- Optimizar estrategias de marketing para mejorar la rentabilidad y eficiencia de futuras campañas

#### Lenguaje de programación, librerías y habilidades 
![Python](https://img.shields.io/badge/PYTHON-%232A5D9F.svg?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/PANDAS-%232A5D9F.svg?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NUMPY-%232A5D9F.svg?style=for-the-badge&logo=numpy&logoColor=white)
![SciPy](https://img.shields.io/badge/SCIPY-%232A5D9F.svg?style=for-the-badge&logo=scipy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/MATPLOTLIB-%232A5D9F.svg?style=for-the-badge&logo=plotly&logoColor=white)
![Seaborn](https://img.shields.io/badge/SEABORN-%232A5D9F.svg?style=for-the-badge&logo=seaborn&logoColor=white)
![Limpieza de Datos](https://img.shields.io/badge/LIMPIEZA%20DE%20DATOS-%233B7DD8.svg?style=for-the-badge&logoColor=white)
![Análisis de Datos](https://img.shields.io/badge/ANÁLISIS%20DE%20DATOS-%233B7DD8.svg?style=for-the-badge&logoColor=white)
![Análisis de Cohortes](https://img.shields.io/badge/ANÁLISIS%20DE%20COHORTES-%233B7DD8.svg?style=for-the-badge&logoColor=white)
![Visualización de Datos](https://img.shields.io/badge/VISUALIZACIÓN%20DE%20DATOS-%233B7DD8.svg?style=for-the-badge&logoColor=white)

#### Preguntas clave
- ¿Cuántas personas usan el sitio web diariamente, semanalmente y mensualmente?

- ¿Qué canales de adquisición generan clientes con mayor LTV?

- ¿Qué combinación de fuente más dispositivo muestra mejor rendimiento?

- ¿Qué métricas son determinantes para decidir en qué canales se debe invertir?
  
#### Metodología 
- **Preprocesamiento de datos:** Se limpiaron y ajustaron los datos: se corrigieron tipos, se eliminaron duplicados y se trataron valores faltantes.

- **Análisis del Comportamiento de Usuarios:** Se estudiaron métricas clave como Usuarios Activos Diarios (DAU), Usuarios Activos Semanales (WAU) y Usuarios Activos Mensuales (MAU), así como la duración promedio de las sesiones y la frecuencia de retorno de los usuarios, para comprender cómo interactúan con la plataforma.

- **Análisis de Ventas:** Se evaluó el momento en que los usuarios comienzan a comprar, el tamaño promedio de compra, el número de pedidos por cliente y el Valor de Vida del Cliente (LTV), con el fin de identificar patrones de consumo.

- **Evaluación de Estrategias de Marketing:** Se calcularon métricas como el Costo de Adquisición de Clientes (CAC), el Retorno de la Inversión en Marketing (ROMI) y los costos por fuente de adquisición, para identificar los canales más rentables y orientar la toma de decisiones estratégicas.

#### Conclusión general
El análisis realizado permitió evaluar las estrategias de marketing con base en métricas clave como el CAC (Costo de Adquisición de Clientes), el ROMI (Retorno de la Inversión en Marketing) y el LTV (Valor del Ciclo de Vida del Cliente). Estas métricas revelaron insights sólidos para la optimización de campañas y asignación de presupuesto.

#### Recomendaciones
- Fuente 1: por su estabilidad y eficiencia, ideal para estrategias sostenidas a largo plazo.

- Fuente 2: por su consistencia en resultados y bajo CAC, representa una inversión inteligente y continua.

- Fuente 4: puede ser rentable en periodos de alta demanda, pero requiere seguimiento constante para asegurar que su alto CAC se compense con un LTV favorable.

Es clave diversificar la inversión entre fuentes estables y fuentes de alto impacto, adaptando la estrategia a las condiciones del mercado. Mientras el LTV se mantenga elevado, es válido invertir incluso en canales con CAC más alto, siempre que el ROMI siga siendo positivo.

#### Diccionario de datos

La tabla `visits` (registros del servidor con datos sobre las visitas al sitio web):

- `Uid:` identificador único del usuario.

- `Device:` dispositivo del usuario.

- `Start Ts:` fecha y hora de inicio de la sesión.

- `End Ts:` fecha y hora de término de la sesión.

- `Source Id:` identificador de la fuente de anuncios de la que proviene el usuario.

Todas las fechas de esta tabla están en formato `AAAA-MM-DD`.

La tabla `orders` (datos sobre pedidos):

- `Uid:` identificador único del usuario que realiza un pedido.

- `Buy Ts:` fecha y hora del pedido. Revenue: el ingreso de Showz por el pedido.

La tabla `costs` (datos sobre gastos de marketing):

- `source_id:` identificador de la fuente de anuncios.

- `dt:` fecha.

- `costs:` gastos en esta fuente de anuncios en este día.

