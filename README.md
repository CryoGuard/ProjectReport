<div class="cover" align="center">
  <img src="https://upload.wikimedia.org/wikipedia/commons/f/fc/UPC_logo_transparente.png"/><br>
  <p><strong>Universidad Peruana de Ciencias Aplicadas</strong></p>
  <p>
  Ingeniería de Software <br><br>
  Periodo: 202610 <br><br>
  1ASI0572 Desarrollo de Soluciones IOT <br><br>
  NCR: 6772 <br><br>
  Docente: Marco Antonio Leon Baca <br><br>
  Informe de Trabajo Final <br><br>
  StartUp: CryoGuard <br><br>
  Producto: CryoGuard Pro <br><br>
  </p>
  <table align="center">
    <tr>
      <th>Member</th>
      <th>Code</th>
    </tr>
    <tr>
      <td>Arias Segil, Marllely Anahi</td>
      <td>U202223984</td>
    </tr>
    <tr>
      <td>Hallasi Saravia, Miguel</td>
      <td>U202312391</td>
    </tr>
    <tr>
      <td>Miranda Ayasta, Rogger Faryd</td>
      <td>U202319239</td>
    </tr>
    <tr>
      <td>Sanchez Rios, Camila</td>
      <td>U202210973</td>
    </tr>
    <tr>
      <td>Vargas Javier, Jose Enrique</td>
      <td>U20221F693</td>
    </tr>
  </table>
  <br><br>
Abril 2026
</div>

## 3.1. User Stories

Las User Stories son clave en metodologías ágiles porque traducen los requisitos funcionales desde la mirada del usuario. Cada historia especifica una necesidad concreta, lo que permite planificar, priorizar y construir el sistema de forma iterativa. Así se asegura que cada función aporte valor real y permanezca alineada con las expectativas del usuario final.

<!-- US01 -->
<table border="1" cellspacing="0" cellpadding="8">
  <tr>
    <th>Story ID</th>
    <th>User</th>
    <th>Priority</th>
    <th>Epic</th>
  </tr>
  <tr>
    <td>US01</td>
    <td>Operador de transporte</td>
    <td>Alta</td>
    <td>EP01 - Monitoreo y Control del Contenedor Inteligente</td>
  </tr>

  <tr>
    <th>Title</th>
    <td colspan="3">Monitorear temperatura en tiempo real	</td>
  </tr>

  <tr>
    <th colspan="4">Description</th>
  </tr>
  <tr>
    <td colspan="4">
      Como operador de transporte, quiero monitorear la temperatura del contenedor en tiempo real durante todo el trayecto, para asegurar que las vacunas y medicamentos se mantengan dentro del rango permitido.
    </td>
  </tr>

  <tr>
    <th colspan="4">Acceptance Criteria</th>
  </tr>
  <tr>
    <td colspan="4">
      <p><strong>Escenario 01: Temperatura dentro del rango permitido</strong></p>
      <ul>
        <li>Dado que el sensor de temperatura registra valores dentro del rango configurado,</li>
        <li>Cuando el sistema procesa los datos,</li>
        <li>Entonces el LED se mantiene en color verde</li>
        <li>Y no se activan alertas sonoras.</li>
      </ul>
        <p><strong>Escenario 02: Temperatura fuera del rango permitido</strong></p>
      <ul>
        <li>Dado que el sensor de temperatura registra valores fuera del rango configurado,</li>
        <li>Cuando el sistema detecta la desviación,</li>
        <li>Entonces se activa LED rojo y buzzer</li>
        <li>Y se genera un flag crítico en el sistema.</li>
      </ul>
    </td>
  </tr>
</table>

<!-- US02 -->

<table border="1" cellspacing="0" cellpadding="8">
  <tr>
    <th>Story ID</th>
    <th>User</th>
    <th>Priority</th>
    <th>Epic</th>
  </tr>
  <tr>
    <td>US02</td>
    <td>Operador de transporte</td>
    <td>Alta</td>
    <td>EP01 - Monitoreo y Control del Contenedor Inteligente</td>
  </tr>

  <tr>
    <th>Title</th>
    <td colspan="3">Monitorear humedad del contenedor</td>
  </tr>

  <tr>
    <th colspan="4">Description</th>
  </tr>
  <tr>
    <td colspan="4">
      Como operador de transporte, quiero monitorear los niveles de humedad dentro del contenedor, para evitar que la humedad excesiva dane los productos biomedicos sensibles.
    </td>
  </tr>

  <tr>
    <th colspan="4">Acceptance Criteria</th>
  </tr>
  <tr>
    <td colspan="4">
      <p><strong>Escenario 01: Humedad dentro del rango permitido</strong></p>
      <ul>
        <li>Dado que el sensor de humedad registra valores dentro del rango configurado (30%-70%),</li>
        <li>Cuando el sistema procesa los datos,</li>
        <li>Entonces no se genera ninguna alerta relacionada con humedad,</li>
        <li>Y el sistema mantiene el estado normal del envio.</li>
      </ul>
      <p><strong>Escenario 02: Humedad fuera del rango permitido</strong></p>
      <ul>
        <li>Dado que el sensor de humedad registra valores por debajo o por encima del rango,</li>
        <li>Cuando el sistema detecta la desviacion,</li>
        <li>Entonces se activa un flag preventivo,</li>
        <li>Y se envia una notificacion a la app del supervisor.</li>
      </ul>
    </td>
  </tr>
</table>

<!-- US03 -->
<table border="1" cellspacing="0" cellpadding="8">
  <tr>
    <th>Story ID</th>
    <th>User</th>
    <th>Priority</th>
    <th>Epic</th>
  </tr>
  <tr>
    <td>US03</td>
    <td>Operador de transporte</td>
    <td>Media</td>
    <td>EP01 - Monitoreo y Control del Contenedor Inteligente</td>
  </tr>
<div class="page"/>

<div class="Student-Outcome">

# Student Outcome

ABET – EAC - Student Outcome 4

**Criterio:** Capacidad de reconocer responsabilidades éticas y profesionales en situaciones de ingeniería y hacer juicios informados, considerando el impacto de las soluciones en contextos globales, económicos, ambientales y sociales.

<table>
  <tr>
    <td><b>Criterio específico</b></td>
    <td><b>Acciones realizadas</b></td>
    <td><b>Conclusiones</b></td>
  </tr>
  <tbody>
    <tr>
      <td><b>Reconoce responsabilidad ética y profesional en situaciones de ingeniería de software</b></td>
      <td>
        <p><b>Miranda Ayasta, Rogger Faryd</b></p>
        <p><b>AV1: </b> </p>
        <p><b>TB1: </b> </p>
        <p><b>AV2: </b> </p>
        <p><b>TB2: </b> </p>
        <p><b>Vargas Javier, Jose Enrique</b></p>
        <p><b>AV1: </b> </p>
        <p><b>TB1: </b> </p>
        <p><b>AV2: </b> </p>
        <p><b>TB2: </b> </p>
        <p><b>Sanchez Rios, Camila</b></p>
        <p><b>AV1: </b> </p>
        <p><b>TB1: </b> </p>
        <p><b>AV2: </b> </p>
        <p><b>TB2: </b> </p>
        <p><b>Arias Segil, Marllely Anahi</b></p>
        <p><b>AV1: </b>Al diseñar la arquitectura y los modelos como el EventStorming o el Context Mapping, traté de asegurar que el sistema sea confiable, que permita monitoreo en tiempo real y que reduzca errores humanos. También consideré aspectos como la disponibilidad, la precisión de los datos y la capacidad de funcionar incluso sin conexión.</p>
        <p><b>TB1: </b> </p>
        <p><b>AV2: </b> </p>
        <p><b>TB2: </b> </p>
        <p><b>Apellidos y Nombres</b></p>
        <p><b>AV1: </b> </p>
        <p><b>TB1: </b> </p>
        <p><b>AV2: </b> </p>
        <p><b>TB2: </b> </p>
      </td>
      <td></td>
    </tr>
  </tbody>
</table>

</div>

<div class="page"/>

<div class="chap1">

# Capítulo I: Introducción

## 1.1. Startup Profile

### 1.1.1. Descripción de la Startup

<h6> Nombre del Startup: CryoGuard </h6>

CryoGuard es una plataforma de logística predictiva diseñada para reducir significativamente las pérdidas en la cadena de frío de productos biomédicos y vacunas. Mientras que las soluciones estándar se limitan a reportar daños cuando ya es tarde, CryoGuard combina sensores de alta precisión con Edge Computing para auditar variables críticas (temperatura, vibración, aperturas) y predecir desviaciones térmicas antes de que comprometan el producto.

Diseñado para rutas complejas, el hardware cuenta con una autonomía energética extendida para trayectos prolongados y capacidad de almacenamiento offline para más de 50,000 registros, minimizando la pérdida de trazabilidad incluso en entornos sin conectividad en zonas sin cobertura. Al recuperar la conectividad, el sistema sincroniza la data automáticamente. Nuestra solución permite a centros de salud y operadores logísticos transformar su cadena de frío de reactiva a proactiva, asegurando el cumplimiento normativo y salvando inventarios críticos.

###### **Visión**

Visualizamos una logística sanitaria de 'mínimas pérdidas' en América Latina. Nuestra visión es que la tecnología predictiva de CryoGuard se convierta en el estándar que garantice la integridad de los productos transportados y tratamientos críticos. Transformaremos un sistema vulnerable en una red altamente confiable y totalmente auditable, asegurando que cada suministro llegue viable a su destino, sin importar los desafíos geográficos o la falta de conectividad.

###### **Misión**

Nuestra misión es blindar la cadena de frío del sector salud transformando datos en acciones preventivas. Proveemos a operadores logísticos y centros médicos trazabilidad altamente auditable y analítica predictiva para erradicar las mermas por fluctuaciones térmicas, garantizar el estricto cumplimiento normativo y asegurar la calidad clínica de cada envío.

### 1.1.2. Perfiles de integrantes del equipo

  <tr>
    <th>Title</th>
    <td colspan="3">Detectar vibraciones o impactos</td>
  </tr>

  <tr>
    <th colspan="4">Description</th>
  </tr>
  <tr>
    <td colspan="4">
      Como operador de transporte, quiero detectar vibraciones o impactos anormales durante el traslado, para identificar si los productos han sufrido golpes que puedan comprometer su integridad.
    </td>
  </tr>

  <tr>
    <th colspan="4">Acceptance Criteria</th>
  </tr>
  <tr>
    <td colspan="4">
      <p><strong>Escenario 01: Vibracion dentro del umbral normal</strong></p>
      <ul>
        <li>Dado que el sensor de vibracion registra valores dentro del umbral normal,</li>
        <li>Cuando el sistema evalua los datos,</li>
        <li>Entonces no se genera ningun flag,</li>
        <li>Y el envio continua sin incidentes de impacto.</li>
      </ul>
      <p><strong>Escenario 02: Vibracion que supera el umbral permitido</strong></p>
      <ul>
        <li>Dado que el sensor de vibracion registra un impacto o vibracion excesiva,</li>
        <li>Cuando el sistema detecta la anomalia,</li>
        <li>Entonces se registra el evento con timestamp,</li>
        <li>Y se anade al log de incidentes del envio.</li>
      </ul>
    <th>
      <img src="img/.jpg" width="800px">
    </th>
    <td valign="top">
      <p><b>Miguel Angel Hallasi</b></p>
      <p>Estudiante del séptimo ciclo, motivado por el aprendizaje continuo y la adquisición de nuevas experiencias en desarrollo móvil, diseño de interfaces y trabajo colaborativo.</p>
    </td>
  </tr>
  <tr>
    <th>
      <img src="img/marlle.png" width="800px">
    </th>
    <td valign="top">
      <p><b>Marllely Anahi Arias Segil</b></p>
      <p>Hola, mi nombre es Marllely Arias Segil. Soy estudiante 
      de Ingeniería de Software en la Universidad Peruana de 
      Ciencias Aplicadas (UPC), una persona empática, 
      responsable y comprometida con mi crecimiento 
      profesional. Me gusta trabajar en equipo y siempre busco 
      dar lo mejor de mí en cada proyecto. </p>
    </td>
  </tr>
</table>

<!-- US04 -->
<table border="1" cellspacing="0" cellpadding="8">
  <tr>
    <th>Story ID</th>
    <th>User</th>
    <th>Priority</th>
    <th>Epic</th>
  </tr>
  <tr>
    <td>US04</td>
    <td>Supervisor de logistica</td>
    <td>Alta</td>
    <td>EP01 - Monitoreo y Control del Contenedor Inteligente</td>
  </tr>
## 1.2. Solution Profile

###### **Descripción General de la Solución**

CryoGuard es una plataforma de inteligencia operativa que transforma el transporte de productos médicos en un proceso predictivo y altamente auditable. En lugar de simplemente registrar datos, nuestro sistema procesa variables críticas (temperatura, aperturas, geolocalización) directamente en el dispositivo (Edge Computing) para detectar tendencias de riesgo térmico antes de que se materialice una falla.

Al detectar un riesgo inminente, CryoGuard detona protocolos de rescate en tiempo real (como alertas predictivas a los conductores y notificaciones de emergencia al centro de control) permitiendo decisiones operativas inmediatas que previenen la pérdida del lote. Diseñada para operar ininterrumpidamente, la solución garantiza una trazabilidad continua y verificable incluso en rutas sin cobertura celular, asegurando a operadores logísticos y centros de salud un cumplimiento normativo estricto y la mayor probabilidad de conservar la viabilidad de los envíos.

###### **Características Clave de la Solución**

- **Inteligencia Predictiva Offline (Edge Computing):** Análisis de riesgos térmicos procesados directamente en el dispositivo, sin depender de la nube, mediante evaluación de umbrales dinámicos y análisis de tendencias en series temporales (variación de temperatura en el tiempo).
  
Problema que resuelve: Evita que la carga se pierda al atravesar zonas sin cobertura celular. Al detectar un riesgo, el dispositivo no espera a tener internet; toma la decisión inmediata de detonar protocolos de rescate locales (como alertar al chofer) antes de que el daño sea irreversible.

- **Trazabilidad:** Almacenamiento redundante y encriptado en memoria física que registra cada segundo del historial del viaje.

Problema que resuelve: Elimina los "puntos ciegos" de auditoría. Garantiza a las autoridades sanitarias y laboratorios un alto nivel de cumplimiento normativo, asegurando que la data histórica del producto se preserve incluso ante fallos de conectividad, incluso si el vehículo sufre un apagón total de comunicaciones.

- **Auditoría Ambiental Integral:** Monitoreo cruzado de temperatura, humedad y vibraciones físicas excesivas (baches severos, caídas).
  
Previene el rechazo de lotes no solo por estrés térmico, sino por estrés mecánico. Identifica si la mala manipulación del transportista antes de que se materialice una ruptura de la cadena de frío, permitiendo deslindar responsabilidades económicas de manera exacta.

- **Geolocalización Cruzada con Tiempos Térmicos** Monitoreo GPS y geocercas sincronizadas con la capacidad de retención de frío del empaque modelada en función del tipo de empaque térmico y condiciones ambientales.

Detecta desvíos, paradas no autorizadas o tráfico pesado que amenazan el límite de tiempo del empaque térmico. Esto permite a la central logística redireccionar la carga a un puerto seguro cercano antes de que el hielo seco o gel refrigerante se agote.

- **Triaje de Alertas de Intervención Rápida:** Escalamiento de alarmas a dos niveles: físicas (visual/sonora para el operador local) y digitales (centro de control).

Empodera al chofer para tomar acciones correctivas inmediatas (ej. revisar el cierre del contenedor en la cabina). Al mismo tiempo, evita la "fatiga de notificaciones" en la central logística, enviando reportes a la nube únicamente cuando la desviación es crítica y requiere intervención remota.

###### **Beneficios de la Solución**

- **Intervención Preventiva:** Gracias al procesamiento en el borde (Edge Computing), el sistema alerta sobre tendencias de riesgo térmico con anticipación suficiente para intervención operativa de que se rompa la cadena de frío, permitiendo la intervención física del transportista o el desvío de la ruta para salvar el lote antes de que ocurra el daño.
  
- **Cumplimiento Normativo:** El almacenamiento local resistente a pérdida de datos y con integridad verificable garantiza una bitácora forense de cada viaje. Esto permite a laboratorios y centros de salud demostrar ante las autoridades regulatorias que no se evidencian desviaciones críticas en las condiciones del transporte, eliminando el riesgo de demandas o rechazo de lotes por falta de evidencia.

- **Visibilidad Logística:** Al combinar almacenamiento offline con sincronización en la nube, el sistema asegura la recuperación total de la trazabilidad. Las centrales logísticas eliminan el estrés de perder de vista sus activos críticos al atravesar zonas rurales o geográficamente complejas.

- **Inteligencia Comercial y Optimización de Procesos:** La plataforma transforma el monitoreo crudo en datos estructurados listos para procesos de Business Intelligence. Esto permite a los gerentes logísticos analizar patrones históricos, evaluar objetivamente el rendimiento de sus transportistas y tomar decisiones estratégicas basadas en evidencia dura para optimizar sus redes de distribución.

###### **Tecnología y Arquitectura**

El dispositivo está diseñado para operar con baterías de bajo consumo, optimizando la frecuencia de muestreo y transmisión para maximizar la autonomía durante trayectos prolongados.

La arquitectura de CryoGuard está estructurada en un modelo de tres capas para garantizar un flujo de datos continuo, una latencia mínima en emergencias y una alta disponibilidad de la información:

- **Capa Física y Procesamiento**
El hardware está compuesto por un microcontrolador de bajo consumo integrado con un arreglo de sensores (temperatura, humedad, acelerómetro y magnético de apertura). Aquí reside nuestro motor de Edge Computing: en lugar de ser un simple transmisor, el dispositivo ejecuta localmente algoritmos de evaluación de umbrales.

Las decisiones que toma: Si las variables superan los límites configurados, el sistema no espera a tener internet; detona acciones autónomas inmediatas, como activar alarmas físicas (buzzer y LEDs) para el transportista y registrar el evento crítico en su memoria interna no volátil. Esto asegura una auditoría forense ininterrumpida incluso en zonas sin cobertura celular.

- **Capa de Red y Backend**
Actúa como el motor de ingesta y orquestación de datos. Cuando el dispositivo detecta una red disponible (vía módulo celular o protocolos IoT), empaqueta el historial almacenado offline y lo transmite de forma segura hacia nuestra infraestructura en la nube.

El flujo de datos: El backend recibe la telemetría cruda, valida la integridad de los paquetes y procesa la información en bases de datos relacionales y de series temporales. Un motor de reglas en la nube clasifica la severidad de los eventos y se encarga de disparar webhooks o correos electrónicos de emergencia a los centros de control logístico.

- **Capa de Aplicación e Inteligencia Comercial**
Es la interfaz donde los datos estructurados se transforman en estrategia operativa. A través de aplicaciones web y móviles, los clientes acceden a la plataforma para interactuar con la información.

El impacto visual: Los operadores logísticos visualizan dashboards dinámicos que muestran el estado de la flota en tiempo real, rastreo por geolocalización y el estatus térmico de cada contenedor. El sistema incluye herramientas de análisis de datos para generar reportes de cumplimiento normativo y métricas de rendimiento, permitiendo a los gerentes optimizar rutas y evaluar la eficiencia de su red de distribución basándose en datos concretos.

### 1.2.1. Antecedentes y problemática

Mediante la técnica de “5W's & 2H’s”, se han identificado los antecedentes y la problemática relacionados con el transporte de vacunas y medicamentos sensibles a la temperatura, lo cual ha motivado el desarrollo de CryoGuard como una solución tecnológica orientada a fortalecer la cadena de frío.

###### **What? (¿Qué?)**

La pérdida de eficacia, viabilidad y el consecuente descarte masivo de productos biomédicos (vacunas y medicamentos termosensibles) debido a rupturas en la cadena de frío y daños mecánicos no detectados durante el transporte logístico.

###### **When? (¿Cuándo?)**

El problema se materializa en los "puntos ciegos" operativos: durante las transferencias de carga, retrasos imprevistos por tráfico o retenes, y en los últimos kilómetros de trayectos largos donde la autonomía de los empaques térmicos pasivos se agota antes de llegar a su destino.

###### **Where? (¿Dónde?)**

En rutas de transporte interprovincial y rural que atraviesan geografías complejas (cambios drásticos de altitud y microclimas), especialmente en zonas de América Latina donde la topografía y la falta de cobertura celular impiden la transmisión de alertas de auxilio cuando el vehículo falla.

###### **Who? (¿Quién?)**

Los actores que asumen el costo logístico y financiero: laboratorios farmacéuticos productores, operadores logísticos tercerizados (3PL) que enfrentan penalidades contractuales, y entidades del Estado (Ministerios de Salud) o clínicas privadas que pierden capacidad de atención médica.

###### **Why? (¿Por qué?)**

Por la dependencia de metodologías de auditoría reactivas ("post-mortem"). La industria utiliza data loggers básicos que solo revelan el historial de temperatura al final del viaje, lo que imposibilita la toma de decisiones estratégicas o el rescate de la carga mientras el vehículo aún está en ruta.

###### **How? (¿Cómo?)**

El quiebre de la cadena de frío ocurre por fallos en los sistemas de refrigeración de los camiones (apagados de motor), aperturas de puertas no autorizadas que liberan la temperatura óptima, exposición prolongada al clima externo durante las descargas, y estrés físico por vibraciones severas en carreteras en mal estado que generan micro-roturas en los viales.

###### **How much? (¿Cuánto?)**

El impacto financiero y sanitario es masivo. Según datos de la Organización Mundial de la Salud (OMS), hasta el 50% de las vacunas en contextos con infraestructura limitada a nivel mundial pueden perderse debido a fallas logísticas y de control de temperatura. A nivel financiero, estudios de inteligencia comercial (como IQVIA) estiman que la industria biofarmacéutica pierde más de $35,000 millones de dólares anuales por fallas en la cadena de frío, sin contar los costos ocultos de logística inversa para desechar los materiales biopeligrosos dañados.

### 1.2.2. Lean UX Process

#### 1.2.2.1. Lean UX Problem Statements

- **Usuario (Operador en ruta)**

El evento: Falla técnica del camión o estrés térmico en pleno tránsito.

La limitación: Carencia de notificaciones locales (en cabina) en tiempo real.

La consecuencia: Entrega de medicamentos inservibles.

Declaración Lean UX: > "Durante una caída de temperatura o impacto físico en ruta, el operador carece de alertas inmediatas en cabina, lo que le impide accionar protocolos de rescate a tiempo y resulta en la entrega de medicamentos irreversiblemente dañados."

- **Administrador (Gerente Logístico o de Salud)**

El evento: Gestión simultánea de múltiples envíos en zonas de conectividad variable.

La limitación: Dependencia de data loggers reactivos (post-viaje) o pérdida de señal.

La consecuencia: Incapacidad de decisión y pérdida financiera.

Declaración Lean UX: > "Al supervisar múltiples rutas, el administrador sufre puntos ciegos de trazabilidad y retraso en la recepción de datos, lo que le impide desviar unidades en peligro y genera pérdidas económicas por penalidades o descarte de inventario."

#### 1.2.2.2. Lean UX Assumptions

- **Business Outcomes**

Hipótesis de Reducción de Mermas: Creemos que al transicionar de un monitoreo reactivo a uno predictivo, nuestros clientes reducirán sus pérdidas económicas por descarte de medicamentos en al menos con un objetivo inicial de reducción del 30–40%.

Hipótesis de Retención/Ventas: Creemos que al garantizar una trazabilidad completa en condiciones operativas normales auditable (cero puntos ciegos), los operadores logísticos podrán ganar más licitaciones con el Estado o grandes farmacéuticas.

- **Users**

Operador de transporte (Chofer): Conduciendo en rutas de topografía compleja, sin señal celular y con alta carga de estrés al volante.

Administrador Logístico (Central): Supervisando simultáneamente decenas de unidades en tránsito, abrumado por notificaciones y con presión por evitar penalidades económicas.

- **Users Outcomes & Benefits**

Intervención Temprana: Si proporcionamos predicciones de riesgo térmico en la plataforma web, entonces el administrador logístico podrá desviar la unidad al centro de salud más cercano antes de que la cadena de frío se rompa.

Seguridad Forense: Si entregamos un reporte automatizado resistente a pérdida de datos y con integridad verificable al finalizar el viaje, entonces el personal de la clínica receptora firmará la conformidad del lote en segundos, sin temor a responsabilidades legales.

- **Feature Assumptions**

Hipótesis del Edge Computing y Alarmas Físicas (LED/Buzzer): Creemos que si el dispositivo detona una alarma sonora fuerte en la cabina al detectar una caída térmica offline, entonces el chofer se detendrá inmediatamente a revisar el cierre del contenedor, salvando la carga.

Hipótesis del Sensor de Apertura: Creemos que si cruzamos el sensor magnético de apertura con el GPS, entonces el administrador podrá diferenciar instantáneamente entre una falla técnica del camión y un intento de robo o sabotaje en ruta.

Hipótesis del Almacenamiento Offline: Creemos que si el dispositivo guarda la data localmente en zonas rurales y la sincroniza al recuperar red, entonces eliminaremos los rechazos de lotes médicos causados por "falta de datos" en la auditoría final.

- **Business Assumptions**

Hipótesis de Valor: Creemos que las empresas logísticas están dispuestas a pagar una suscripción premium (SaaS/HaaS) por CryoGuard, porque el costo mensual de nuestra plataforma es marginal comparado con el costo de perder un solo lote de vacunas especializadas.

Hipótesis de Cumplimiento: Asumimos que las nuevas normativas sanitarias obligarán a todas las clínicas a exigir trazabilidad ininterrumpida, convirtiendo a CryoGuard de un "lujo tecnológico" a una necesidad regulatoria.

- **User Assumptions**

Fricción Tecnológica Cero: Asumimos que el personal médico no tiene tiempo ni conocimientos técnicos; por lo tanto, si el dispositivo requiere "emparejamiento Bluetooth manual" o configuraciones complejas, no lo usarán. Debe ser de encendido automático al cerrar la caja.

Fatiga de Alarmas: Asumimos que si enviamos notificaciones a la central por cada variación mínima de temperatura, el administrador las ignorará. Por ello, la nube solo debe alertar cuando el algoritmo detecte un riesgo inminente de daño.

#### 1.2.2.3. Lean UX Hypothesis Statements

Creemos que al dotar a los operadores de transporte médico con herramientas de Edge Computing y alertas predictivas en cabina, lograremos que intervengan proactivamente antes de que ocurra una ruptura térmica, incrementando la probabilidad de mantener la viabilidad de los tratamientos críticos durante su trayecto.

Sabremos que la solución es efectiva y el modelo de negocio es viable cuando, tras los primeros pilotos, comprobemos empíricamente que:

- Tasa de Intervención Temprana: El operador atiende y reacciona a las alertas físicas (LED/Buzzer) en la cabina en un tiempo menor a 15 minutos, evitando la exposición prolongada del producto.

- Reducción de Mermas: Logramos un objetivo inicial de reducción del 30–40%, en la tasa de rechazo de lotes o pérdida total de inventario atribuible a fluctuaciones térmicas en las rutas monitoreadas.

- Integridad de la Trazabilidad: Alcanzamos un 99.9% de recuperación de datos históricos al finalizar los viajes, demostrando que el almacenamiento offline elimina los puntos ciegos causados por las zonas sin cobertura celular.

- Eficiencia en el Centro de Control: Disminuimos en una reducción significativa el volumen de falsas alarmas o notificaciones irrelevantes recibidas por el administrador, demostrando que el triaje de alertas funciona correctamente.

- Cumplimiento Normativo: La mayoría de los viajes completados generan automáticamente un reporte forense resistente a pérdida de datos y con integridad verificable aceptado por los centros de salud receptores sin disputas legales.

#### 1.2.2.4. Lean UX Canvas

<img src="img/ux.JPG" width="800px">

## 1.3. Segmentos objetivo

###### Redes de Centros de Salud (Urbanos y Rurales)

Nos dirigimos a las entidades administrativas (privadas o públicas) encargadas de abastecer y gestionar clínicas, hospitales y postas médicas, garantizando que el inventario farmacéutico llegue viable desde la central hasta el punto de atención final.

- Tamaño: Redes de salud medianas a grandes, que administran desde 10 hasta decenas de puntos de atención distribuidos en distintas geografías y que realizan despachos de medicamentos recurrentes.

- Capacidad Económica: Presupuestos institucionales (financiación estatal en el sector público o corporativa en el privado). Su disposición de pago se justifica al comparar el costo de la plataforma CryoGuard frente al alto costo de desechar lotes de vacunas por fallas en sus propios traslados internos.

- Nivel Tecnológico: Altamente asimétrico. En la central urbana (donde están los administradores) cuentan con conectividad estable y personal capaz de usar dashboards web. Sin embargo, en los puntos de destino (rurales) el personal médico carece de formación técnica y la conectividad es nula. Por ello, requieren que el dispositivo sea autónomo y no requiera configuraciones complejas por parte del usuario final.

###### ONGs y Gestores de Logística Sanitaria Humanitaria

Nos enfocamos en organizaciones dedicadas a la planificación y ejecución de campañas de salud, distribución de ayuda médica y programas de inmunización en zonas vulnerables o de difícil acceso.

- Tamaño: Operaciones de alcance regional, nacional o internacional que movilizan altos volúmenes de tratamientos médicos críticos durante campañas de salud o respuestas a emergencias.

- Capacidad Económica: Sus presupuestos provienen de fondos de cooperación internacional, donaciones o subvenciones. Son muy estrictos con el gasto, pero tienen la obligación legal y moral de garantizar a sus donantes que la ayuda llega en estado óptimo, lo que hace viable la inversión en trazabilidad.

- Nivel Tecnológico: Acostumbrados a operar en condiciones de infraestructura extrema. Necesitan tecnología de despliegue rápido. Sus centrales requieren datos precisos y reportes automatizados para justificar el uso de fondos, mientras que sus operadores en campo dependen de las alertas físicas del dispositivo y del almacenamiento offline debido a la falta total de red celular en sus misiones.

</div>

<div class="page"/>

<div class="chap2">

# Capítulo II: Requirements Elicitation & Analysis

## 2.1. Competidores
### 2.1.1. Análisis competitivo

  <tr>
    <th>Title</th>
    <td colspan="3">Geolocalizar contenedor en tiempo real</td>
  </tr>

  <tr>
    <th colspan="4">Description</th>
  </tr>
  <tr>
    <td colspan="4">
      Como supervisor de logistica, quiero conocer la ubicacion GPS del contenedor en tiempo real, para monitorear que el transporte siga la ruta planificada.
    </td>
  </tr>

  <tr>
    <th colspan="4">Acceptance Criteria</th>
  </tr>
  <tr>
    <td colspan="4">
      <p><strong>Escenario 01: Visualizacion de ubicacion en mapa</strong></p>
      <ul>
        <li>Dado que el contenedor tiene conexion a internet,</li>
        <li>Cuando el supervisor accede al dashboard web,</li>
        <li>Entonces puede ver la ubicacion exacta del contenedor en un mapa interactivo,</li>
        <li>Y validar que este dentro de la ruta esperada.</li>
      </ul>
      <p><strong>Escenario 02: Actualizacion de ubicacion en intervalos regulares</strong></p>
      <ul>
        <li>Dado que el contenedor esta en movimiento,</li>
        <li>Cuando el sistema recibe datos GPS,</li>
        <li>Entonces actualiza la posicion en el mapa cada 30 segundos o segun intervalo configurado,</li>
        <li>Y mantiene trazabilidad continua del trayecto.</li>
      </ul>
    </td>
  </tr>
</table>

<!-- US05 -->
<table border="1" cellspacing="0" cellpadding="8">
  <tr>
    <th>Story ID</th>
    <th>User</th>
    <th>Priority</th>
    <th>Epic</th>
  </tr>
  <tr>
    <td>US05</td>
    <td>Supervisor de logistica</td>
    <td>Alta</td>
    <td>EP01 - Monitoreo y Control del Contenedor Inteligente</td>
  </tr>

  <tr>
    <th>Title</th>
    <td colspan="3">Activar enfriamiento automatico (Peltier)</td>
  </tr>

  <tr>
    <th colspan="4">Description</th>
  </tr>
  <tr>
    <td colspan="4">
      Como supervisor de logistica, quiero que el sistema active automaticamente el enfriamiento (Peltier) cuando la temperatura supere el rango permitido, para proteger los productos sin intervencion manual.
    </td>
  </tr>

  <tr>
    <th colspan="4">Acceptance Criteria</th>
  </tr>
  <tr>
    <td colspan="4">
      <p><strong>Escenario 01: Activacion automatica de enfriamiento</strong></p>
      <ul>
        <li>Dado que la temperatura supera el rango permitido en mas de 1 C,</li>
        <li>Cuando el sistema detecta la condicion,</li>
        <li>Entonces activa el modulo Peltier, disipador y ventilador automaticamente,</li>
        <li>Y protege la integridad de los productos durante el traslado.</li>
      </ul>
      <p><strong>Escenario 02: Desactivacion al normalizar temperatura</strong></p>
      <ul>
        <li>Dado que el enfriamiento esta activo y la temperatura vuelve al rango permitido,</li>
        <li>Cuando se mantiene estable dentro del rango por 2 minutos,</li>
        <li>Entonces el sistema desactiva automaticamente el enfriamiento,</li>
        <li>Y vuelve al modo de monitoreo normal.</li>
      </ul>
    </td>
  </tr>
</table>

<!-- US06 -->
<table border="1" cellspacing="0" cellpadding="8">
  <tr>
    <th>Story ID</th>
    <th>User</th>
    <th>Priority</th>
    <th>Epic</th>
  </tr>
  <tr>
    <td>US06</td>
    <td>Administrador</td>
    <td>Media</td>
    <td>EP01 - Monitoreo y Control del Contenedor Inteligente</td>
  </tr>

  <tr>
    <th>Title</th>
    <td colspan="3">Bloquear apertura del contenedor (Servo)</td>
  </tr>

  <tr>
    <th colspan="4">Description</th>
  </tr>
  <tr>
    <td colspan="4">
      Como administrador, quiero que el sistema bloquee automaticamente la apertura del contenedor cuando se detecte una condicion critica, para evitar que se acceda a productos en estado vulnerable.
    </td>
  </tr>

  <tr>
    <th colspan="4">Acceptance Criteria</th>
  </tr>
  <tr>
    <td colspan="4">
      <p><strong>Escenario 01: Bloqueo automatico por condicion critica</strong></p>
      <ul>
        <li>Dado que se detecta un flag critico (temperatura extrema o apertura no autorizada),</li>
        <li>Cuando el sistema activa la alerta,</li>
        <li>Entonces el servo bloquea fisicamente la apertura del contenedor,</li>
        <li>Y se restringe el acceso hasta autorizacion valida.</li>
      </ul>
      <p><strong>Escenario 02: Desbloqueo por override autorizado</strong></p>
      <ul>
        <li>Dado que el contenedor esta bloqueado por condicion critica,</li>
        <li>Cuando un usuario autorizado ejecuta override mediante boton fisico o app,</li>
        <li>Entonces el sistema desbloquea el contenedor y registra la accion en el log,</li>
        <li>Y deja trazabilidad del evento de desbloqueo.</li>
      </ul>
    </td>
  </tr>
</table>

<!-- US07 -->
<table border="1" cellspacing="0" cellpadding="8">
  <tr>
    <th>Story ID</th>
    <th>User</th>
    <th>Priority</th>
    <th>Epic</th>
  </tr>
  <tr>
    <td>US07</td>
    <td>Operador de transporte</td>
    <td>Alta</td>
    <td>EP02 - Alertas y Notificaciones</td>
  </tr>

  <tr>
    <th>Title</th>
    <td colspan="3">Recibir alerta visual mediante LED</td>
  </tr>

  <tr>
    <th colspan="4">Description</th>
  </tr>
  <tr>
    <td colspan="4">
      Como operador de transporte, quiero recibir alertas visuales mediante LEDs de colores, para identificar rapidamente el estado del contenedor sin necesidad de mirar una pantalla.
    </td>
  </tr>

  <tr>
    <th colspan="4">Acceptance Criteria</th>
  </tr>
  <tr>
    <td colspan="4">
      <p><strong>Escenario 01: LED verde para estado normal</strong></p>
      <ul>
        <li>Dado que todas las variables estan dentro del rango permitido,</li>
        <li>Cuando el sistema evalua las condiciones,</li>
        <li>Entonces el LED se mantiene en color verde fijo,</li>
        <li>Y el operador identifica que no hay riesgo actual.</li>
      </ul>
      <p><strong>Escenario 02: LED rojo para condicion critica</strong></p>
      <ul>
        <li>Dado que al menos una variable critica esta fuera del rango permitido,</li>
        <li>Cuando el sistema detecta la condicion,</li>
        <li>Entonces el LED parpadea en color rojo,</li>
        <li>Y se indica una accion inmediata del operador.</li>
      </ul>
    </td>
  </tr>
</table>

<!-- US08 -->
<table border="1" cellspacing="0" cellpadding="8">
  <tr>
    <th>Story ID</th>
    <th>User</th>
    <th>Priority</th>
    <th>Epic</th>
  </tr>
  <tr>
    <td>US08</td>
    <td>Operador de transporte</td>
    <td>Alta</td>
    <td>EP02 - Alertas y Notificaciones</td>
  </tr>

  <tr>
    <th>Title</th>
    <td colspan="3">Recibir alerta sonora mediante Buzzer</td>
  </tr>

  <tr>
    <th colspan="4">Description</th>
  </tr>
  <tr>
    <td colspan="4">
      Como operador de transporte, quiero recibir alertas sonoras cuando se detecte una condicion critica, para actuar inmediatamente incluso si no estoy mirando el contenedor.
    </td>
  </tr>

  <tr>
    <th colspan="4">Acceptance Criteria</th>
  </tr>
  <tr>
    <td colspan="4">
      <p><strong>Escenario 01: Activacion de buzzer en condicion critica</strong></p>
      <ul>
        <li>Dado que se detecta un flag critico,</li>
        <li>Cuando el sistema activa las alertas,</li>
        <li>Entonces el buzzer emite un sonido intermitente,</li>
        <li>Y el operador es advertido incluso sin contacto visual.</li>
      </ul>
      <p><strong>Escenario 02: Desactivacion manual del buzzer</strong></p>
      <ul>
        <li>Dado que el buzzer esta activo por una condicion critica,</li>
        <li>Cuando el operador presiona el boton fisico de silencio o confirma la alerta en app,</li>
        <li>Entonces el buzzer se desactiva pero el LED rojo continua parpadeando,</li>
        <li>Y la condicion permanece visible hasta normalizarse.</li>
      </ul>
    </td>
  </tr>
</table>

<!-- US09 -->
<table border="1" cellspacing="0" cellpadding="8">
  <tr>
    <th>Story ID</th>
    <th>User</th>
    <th>Priority</th>
    <th>Epic</th>
  </tr>
  <tr>
    <td>US09</td>
    <td>Supervisor de logistica</td>
    <td>Alta</td>
    <td>EP02 - Alertas y Notificaciones</td>
  </tr>

  <tr>
    <th>Title</th>
    <td colspan="3">Detectar salida de geocerca</td>
    <th>Entrevista</th>
    <td>1</td>
    <th>Nombre</th>
    <td>Gabriel</td>
  </tr>

  <tr>
    <th colspan="4">Description</th>
  </tr>
  <tr>
    <td colspan="4">
      Como supervisor de logistica, quiero recibir una alerta cuando el contenedor salga de la ruta o geocerca definida, para identificar desviaciones no planificadas.
    <th>Edad</th>
    <td>24</td>
    <th>Distrito</th>
    <td>Surco</td>
  </tr>
  <tr>
    <th>Captura de la entrevista: <img src="img/SEG1_1.JPG" alt="Captura de la entrevista" width="250"></th>
    <td colspan="3">
        El entrevistado señala que el principal desafío es la falta de monitoreo en tiempo real, lo que impide actuar ante cambios de temperatura. Además, la conectividad limitada y los retrasos dificultan mantener la cadena de frío. En general, necesita una solución confiable, simple y con capacidad offline que permita alertas inmediatas y evite pérdidas.
    </td>
  </tr>
  <tr>
    <th>URL de la grabación</th>
    <td colspan="3">
      <a href="https://drive.google.com/file/d/18YGJLRUubp6IUsQ-dSzeeukcKNFLEuBg/view?usp=sharing">
        Ver grabación
      </a>
    </td>
  </tr>
  <tr>
   <th>Timing</th>
    <td colspan="3">
         5:20 min
    </td>
  </tr>
</table>

<table border="1">
  <tr>
    <th>Entrevista</th>
    <td>2</td>
    <th>Nombre</th>
    <td>Jocelyn</td>
  </tr>
  <tr>
    <th>Edad</th>
    <td>25</td>
    <th>Distrito</th>
    <td>San Isidro</td>
  </tr>
  <tr>
    <th>Captura de la entrevista: <img src="assets/Chapter-2/entrevista2.png" alt="Captura de la entrevista" width="200"></th>
    <td colspan="3">
      La entrevistada comenta que el monitoreo de temperatura se realiza mayormente de forma manual con termómetros digitales. Indica que uno de los principales retos es mantener la temperatura estable durante todo el traslado, especialmente en viajes largos o con altas temperaturas. Señala que han ocurrido pérdidas porque los problemas se detectan recién al final, cuando ya no se puede actuar. A partir de esto, se identifica que el principal problema es la falta de monitoreo en tiempo real, lo que limita la capacidad de reacción y genera pérdidas evitables. Además, destaca la importancia de contar con alertas inmediatas y una solución tecnológica que sea fácil de usar, funcione sin internet y automatice los reportes.
    </td>
  </tr>
  <tr>
    <th>URL de la grabación</th>
    <td colspan="3">
      <a href="https://drive.google.com/file/d/1skLWn8ivYLy6wcLDn1SCJ-1x6XAePs4K/view?usp=sharing">
        Ver grabación
      </a>
    </td>
  </tr>
  <tr>
   <th>Timing</th>
    <td colspan="3">
         6:26 min
    </td>
  </tr>
</table>

<table border="1">
  <tr>
    <th>Entrevista</th>
    <td>3</td>
    <th>Nombre</th>
    <td>Delba</td>
  </tr>
  <tr>
    <th>Edad</th>
    <td>38</td>
    <th>Distrito</th>
    <td> centro de salud en huancayo</td>
  </tr>
  <tr>
    <th>Captura de la entrevista: <img src="assets/Chapter-2/.png" alt="Captura de la entrevista" width="200"></th>
    <td colspan="3">
      La entrevistada, trabajadora de un centro de salud encargada del manejo de vacunas y cadena de frío, explicó que el transporte se realiza manteniendo una temperatura entre 2 y 8 °C mediante termos porta vacunas, paquetes fríos, termómetros y dispositivos como dataloggers para monitorear la temperatura. Señala que el mayor reto está en el transporte hacia zonas frías o rurales, donde los paquetes tardan más en descongelarse y se requiere una mejor preparación previa. Indica que no ha tenido pérdidas importantes por ruptura de cadena de frío, pero considera fundamental recibir alertas en tiempo real cuando la temperatura sale del rango permitido para activar el plan de contingencia, como trasladar las vacunas a otro contenedor seguro. Además, destaca que una solución tecnológica de monitoreo ayudaría a mejorar la seguridad, el control y la conservación adecuada de las vacunas durante todo el proceso.
    </td>
  </tr>

  <tr>
    <th colspan="4">Acceptance Criteria</th>
  </tr>
  <tr>
    <td colspan="4">
      <p><strong>Escenario 01: Alerta por salida de geocerca</strong></p>
      <ul>
        <li>Dado que se ha definido una geocerca para la ruta del envio,</li>
        <li>Cuando el GPS del contenedor detecta que la ubicacion esta fuera de la geocerca,</li>
        <li>Entonces el sistema genera un flag preventivo y envia una notificacion al supervisor,</li>
        <li>Y se activa seguimiento reforzado del trayecto.</li>
      </ul>
      <p><strong>Escenario 02: Registro de desviacion en el log</strong></p>
      <ul>
        <li>Dado que se detecto una salida de geocerca,</li>
        <li>Cuando el supervisor revisa el historial del envio,</li>
        <li>Entonces puede ver el punto exacto de desviacion con timestamp y duracion,</li>
        <li>Y usar la evidencia para analisis posterior.</li>
      </ul>
    <th>URL de la grabación</th>
    <td colspan="3">
      <a href="https://drive.google.com/drive/folders/1iQFGaorB6bw4b1EpuBW3llKa8cVtb8wm?usp=sharing">
        Ver grabación
      </a>
    </td>
  </tr>
  <tr>
   <th>Timing</th>
    <td colspan="3">
         5:32 min
    </td>
  </tr>
</table>

<!-- US10 -->
<table border="1" cellspacing="0" cellpadding="8">
  <tr>
    <th>Story ID</th>
    <th>User</th>
    <th>Priority</th>
    <th>Epic</th>
  </tr>
  <tr>
    <td>US10</td>
    <td>Supervisor de logistica</td>
    <td>Alta</td>
    <td>EP02 - Alertas y Notificaciones</td>
  </tr>

  <tr>
    <th>Title</th>
    <td colspan="3">Detectar apertura no autorizada del contenedor</td>
    <th>Entrevista</th>
    <td>1</td>
    <th>Nombre</th>
    <td>Isabel</td>
  </tr>

  <tr>
    <th colspan="4">Description</th>
  </tr>
  <tr>
    <td colspan="4">
      Como supervisor de logistica, quiero recibir una alerta cuando el contenedor se abra sin autorizacion, para identificar posibles manipulaciones indebidas de los productos.
    <th>Edad</th>
    <td>27</td>
    <th>Distrito</th>
    <td>Miraflores</td>
  </tr>
  <tr>
    <th>Captura de la entrevista: <img src="img/SEG2_1.JPG" alt="Captura de la entrevista" width="250"></th>
    <td colspan="3">
        La entrevistada señala que el principal problema es la falta de monitoreo en tiempo real, ya que la trazabilidad se basa en registros manuales y dataloggers revisados al final. Además, la conectividad limitada y los riesgos en transbordos y retrasos dificultan el control de la cadena de frío. En general, necesita una solución confiable, simple y con capacidad offline que permita alertas inmediatas, trazabilidad completa y reduzca pérdidas.
    </td>
  </tr>

  <tr>
    <th colspan="4">Acceptance Criteria</th>
  </tr>
  <tr>
    <td colspan="4">
      <p><strong>Escenario 01: Alerta por apertura no autorizada</strong></p>
      <ul>
        <li>Dado que el contenedor esta cerrado y el sistema en modo de transporte,</li>
        <li>Cuando se detecta la apertura del contenedor sin un override previo,</li>
        <li>Entonces se activa flag critico, LED rojo, buzzer y notificacion remota,</li>
        <li>Y se registra un evento de seguridad en el sistema.</li>
      </ul>
      <p><strong>Escenario 02: Registro de apertura autorizada</strong></p>
      <ul>
        <li>Dado que un usuario autorizado ejecuta override antes de abrir,</li>
        <li>Cuando se detecta la apertura del contenedor,</li>
        <li>Entonces se registra como apertura autorizada y no se activan alertas,</li>
        <li>Y se conserva la trazabilidad de la autorizacion.</li>
      </ul>
    <th>URL de la grabación</th>
    <td colspan="3">
      <a href="https://drive.google.com/file/d/1xWDeuagEcSr8o8BPUqwS3ZJFU_zf5NOd/view?usp=sharing">
        Ver grabación
      </a>
    </td>
  </tr>
  <tr>
   <th>Timing</th>
    <td colspan="3">
         6:37 min
    </td>
  </tr>
</table>

<table border="1">
  <tr>
    <th>Entrevista</th>
    <td>2</td>
    <th>Nombre</th>
    <td>Godelino</td>
  </tr>
  <tr>
    <th>Edad</th>
    <td>38</td>
    <th>Distrito</th>
    <td>La Victoria</td>
  </tr>
  <tr>
    <th>Captura de la entrevista: <img src="assets/Chapter-2/godelino.png" alt="Captura de la entrevista" width="250"></th>
    <td colspan="3">
        El entrevistado señala que el principal problema es la falta de visibilidad en tiempo real, ya que dependen de registros físicos revisados solo al llegar a destino. Identifica dos puntos críticos de riesgo: el traslado (lluvia, sol, calor del motor) y los centros de salud rurales donde el personal tiene múltiples funciones. Además, la conectividad limitada en zonas alejadas y la ausencia de vista centralizada dificultan el control de la cadena de frío.
    </td>
  </tr>
  <tr>
    <th>URL de la grabación</th>
    <td colspan="3">
      <a href="https://drive.google.com/file/d/12WSxbUw6aKvV3PrSbK8Tdv1vnpI1AXZA/view?usp=sharing">
        Ver grabación
      </a>
    </td>
  </tr>
  <tr>
   <th>Timing</th>
    <td colspan="3">
         10:57 min
    </td>
  </tr>
</table>

<!-- US11 -->
<table border="1" cellspacing="0" cellpadding="8">
  <tr>
    <th>Story ID</th>
    <th>User</th>
    <th>Priority</th>
    <th>Epic</th>
  </tr>
  <tr>
    <td>US11</td>
    <td>Supervisor de logistica</td>
    <td>Alta</td>
    <td>EP03 - Dashboard Web y Aplicacion Movil</td>
  </tr>

  <tr>
    <th>Title</th>
    <td colspan="3">Visualizar dashboard con mapa de envios activos</td>
  </tr>

  <tr>
    <th colspan="4">Description</th>
  </tr>
  <tr>
    <td colspan="4">
      Como supervisor de logistica, quiero visualizar un dashboard web con un mapa que muestre todos los envios activos, para supervisar su ubicacion y estado de manera centralizada.
    </td>
  </tr>
### 2.2.3. Análisis de entrevistas
En base a la recopilación de datos obtenida mediante las entrevistas, se ha realizado el siguiente análisis cualitativo y cuantitativo. Los hallazgos estadísticos sobre sus comportamientos, herramientas actuales, dolores (pains) y necesidades (gains) servirán como fundamento directo para la construcción de los arquetipos (User Personas).

**Segmento 1: Centros de salud rurales o urbanos**

Las tres entrevistas coinciden en que el principal problema es la falta de monitoreo en tiempo real de la temperatura durante el transporte de vacunas, lo que dificulta actuar de forma inmediata ante una posible ruptura de la cadena de frío. Aunque se utilizan termómetros digitales, dataloggers y controles manuales, muchas veces la verificación se realiza al final del traslado, cuando ya no es posible corregir el problema. También se identifican dificultades en zonas rurales por la conectividad limitada, los largos desplazamientos y las condiciones climáticas. Como punto fuerte, todos resaltan la necesidad de una solución tecnológica simple, confiable, con alertas inmediatas, capacidad offline y mejor trazabilidad para prevenir pérdidas y mejorar la seguridad de las vacunas.

**Segmento 2: ONGs y gestores de logística sanitaria**

En este segmento, las entrevistas muestran que el mayor reto está en la falta de visibilidad completa y control en tiempo real de la cadena de frío, ya que gran parte del seguimiento depende de registros manuales o revisiones posteriores. Los riesgos aumentan durante el transporte, especialmente por factores climáticos, transbordos y la carga operativa del personal en centros rurales. Además, la limitada conectividad dificulta el monitoreo constante y la toma de decisiones rápidas. Como punto fuerte, ambos entrevistados destacan la necesidad de una plataforma centralizada, confiable y con funcionamiento offline que permita trazabilidad completa, alertas inmediatas y una mejor gestión logística para reducir pérdidas y optimizar recursos.

</div>

  <tr>
    <th colspan="4">Acceptance Criteria</th>
  </tr>
  <tr>
    <td colspan="4">
      <p><strong>Escenario 01: Mapa con todos los envios activos</strong></p>
      <ul>
        <li>Dado que hay multiples envios en curso,</li>
        <li>Cuando el supervisor accede al dashboard,</li>
        <li>Entonces ve un mapa con marcadores de cada contenedor activo y su estado (verde/normal, amarillo/preventivo, rojo/critico),</li>
        <li>Y puede priorizar acciones sobre los envios criticos.</li>
      </ul>
      <p><strong>Escenario 02: Filtros por region y estado</strong></p>
      <ul>
        <li>Dado que el supervisor quiere enfocarse en una region especifica,</li>
        <li>Cuando aplica filtros por region o estado,</li>
        <li>Entonces el mapa muestra solo los envios que cumplen con los criterios seleccionados,</li>
        <li>Y mejora la supervision operativa por segmento.</li>
      </ul>
    </td>
  </tr>
</table>

<!-- US12 -->
<table border="1" cellspacing="0" cellpadding="8">
  <tr>
    <th>Story ID</th>
    <th>User</th>
    <th>Priority</th>
    <th>Epic</th>
  </tr>
  <tr>
    <td>US12</td>
    <td>Supervisor de logistica</td>
    <td>Alta</td>
    <td>EP03 - Dashboard Web y Aplicacion Movil</td>
  </tr>

  <tr>
    <th>Title</th>
    <td colspan="3">Consultar logs historicos de envios</td>
  </tr>

  <tr>
    <th colspan="4">Description</th>
  </tr>
  <tr>
    <td colspan="4">
      Como supervisor de logistica, quiero consultar los logs historicos de envios anteriores, para analizar incidentes pasados y mejorar rutas futuras.
    </td>
  </tr>

  <tr>
    <th colspan="4">Acceptance Criteria</th>
  </tr>
  <tr>
    <td colspan="4">
      <p><strong>Escenario 01: Visualizacion de historial por envio</strong></p>
      <ul>
        <li>Dado que el supervisor selecciona un envio completado,</li>
        <li>Cuando accede a los detalles del envio,</li>
        <li>Entonces puede ver el log completo de temperatura, humedad, vibracion, ubicacion y eventos de apertura,</li>
        <li>Y analizar incidentes con contexto completo.</li>
      </ul>
      <p><strong>Escenario 02: Exportacion de logs</strong></p>
      <ul>
        <li>Dado que el supervisor necesita compartir los logs con un auditor,</li>
        <li>Cuando selecciona la opcion de exportacion,</li>
        <li>Entonces el sistema genera un archivo CSV o PDF con todos los datos del envio,</li>
        <li>Y facilita auditoria y cumplimiento documental.</li>
      </ul>
    </td>
  </tr>
</table>

<!-- US13 -->
<table border="1" cellspacing="0" cellpadding="8">
  <tr>
    <th>Story ID</th>
    <th>User</th>
    <th>Priority</th>
    <th>Epic</th>
  </tr>
  <tr>
    <td>US13</td>
    <td>Operador de transporte</td>
    <td>Alta</td>
    <td>EP03 - Dashboard Web y Aplicacion Movil</td>
  </tr>

  <tr>
    <th>Title</th>
    <td colspan="3">Recibir notificaciones push en app movil</td>
  </tr>

  <tr>
    <th colspan="4">Description</th>
  </tr>
  <tr>
    <td colspan="4">
      Como operador de transporte, quiero recibir notificaciones push en mi aplicacion movil cuando se detecte una condicion critica, para actuar rapidamente incluso si no estoy cerca del contenedor.
    </td>
  </tr>

  <tr>
    <th colspan="4">Acceptance Criteria</th>
  </tr>
  <tr>
    <td colspan="4">
      <p><strong>Escenario 01: Notificacion push por flag critico</strong></p>
      <ul>
        <li>Dado que se detecta un flag critico en el contenedor,</li>
        <li>Cuando el sistema procesa el evento,</li>
        <li>Entonces envia una notificacion push a la app movil del operador asignado al envio,</li>
        <li>Y permite reaccion inmediata ante el incidente.</li>
      </ul>
      <p><strong>Escenario 02: Contenido de la notificacion</strong></p>
      <ul>
        <li>Dado que el operador recibe la notificacion,</li>
        <li>Cuando abre la app,</li>
        <li>Entonces puede ver que variable causo el flag, el valor registrado y la accion recomendada,</li>
        <li>Y decidir la respuesta operativa adecuada.</li>
      </ul>
    </td>
  </tr>
</table>

<!-- US14 -->
<table border="1" cellspacing="0" cellpadding="8">
  <tr>
    <th>Story ID</th>
    <th>User</th>
    <th>Priority</th>
    <th>Epic</th>
  </tr>
  <tr>
    <td>US14</td>
    <td>Administrador</td>
    <td>Media</td>
    <td>EP03 - Dashboard Web y Aplicacion Movil</td>
  </tr>

  <tr>
    <th>Title</th>
    <td colspan="3">Gestionar usuarios y roles desde dashboard</td>
  </tr>

  <tr>
    <th colspan="4">Description</th>
  </tr>
  <tr>
    <td colspan="4">
      Como administrador, quiero gestionar usuarios y asignar roles desde el dashboard web, para controlar quien tiene acceso a que funcionalidades del sistema.
    </td>
  </tr>

  <tr>
    <th colspan="4">Acceptance Criteria</th>
  </tr>
  <tr>
    <td colspan="4">
      <p><strong>Escenario 01: Crear nuevo usuario</strong></p>
      <ul>
        <li>Dado que el administrador esta en el panel de gestion de usuarios,</li>
        <li>Cuando ingresa nombre, correo y selecciona un rol (Operador, Supervisor, ONG),</li>
        <li>Entonces el sistema crea el usuario y envia un correo con instrucciones de acceso,</li>
        <li>Y deja el registro de alta en el sistema.</li>
      </ul>
      <p><strong>Escenario 02: Modificar rol de usuario existente</strong></p>
      <ul>
        <li>Dado que un usuario cambia de puesto o responsabilidades,</li>
        <li>Cuando el administrador modifica su rol,</li>
        <li>Entonces el sistema actualiza los permisos del usuario sin afectar sus datos historicos,</li>
        <li>Y aplica la nueva politica de acceso de inmediato.</li>
      </ul>
    </td>
  </tr>
</table>

<!-- US15 -->
<table border="1" cellspacing="0" cellpadding="8">
  <tr>
    <th>Story ID</th>
    <th>User</th>
    <th>Priority</th>
    <th>Epic</th>
  </tr>
  <tr>
    <td>US15</td>
    <td>Operador de transporte</td>
    <td>Alta</td>
    <td>EP04 - Almacenamiento y Sincronizacion de Datos</td>
  </tr>

  <tr>
    <th>Title</th>
    <td colspan="3">Almacenar datos localmente durante transporte offline</td>
  </tr>

  <tr>
    <th colspan="4">Description</th>
  </tr>
  <tr>
    <td colspan="4">
      Como operador de transporte, quiero que el sistema almacene todos los datos de sensores localmente cuando no hay conexion a internet, para no perder informacion durante trayectos en zonas sin cobertura.
    </td>
  </tr>

  <tr>
    <th colspan="4">Acceptance Criteria</th>
  </tr>
  <tr>
    <td colspan="4">
      <p><strong>Escenario 01: Almacenamiento automatico en tarjeta SD</strong></p>
      <ul>
        <li>Dado que el contenedor esta en una zona sin conectividad,</li>
        <li>Cuando los sensores capturan datos,</li>
        <li>Entonces el sistema guarda toda la informacion en la memoria interna o tarjeta SD,</li>
        <li>Y evita perdida de datos durante el trayecto.</li>
      </ul>
      <p><strong>Escenario 02: Capacidad de almacenamiento suficiente</strong></p>
      <ul>
        <li>Dado que el trayecto dura hasta 7 dias sin conectividad,</li>
        <li>Cuando el sistema almacena datos continuamente,</li>
        <li>Entonces la tarjeta SD tiene capacidad suficiente para retener todos los datos sin sobrescribir,</li>
        <li>Y conserva la trazabilidad completa del envio.</li>
      </ul>
    </td>
  </tr>
</table>

<!-- US16 -->
<table border="1" cellspacing="0" cellpadding="8">
  <tr>
    <th>Story ID</th>
    <th>User</th>
    <th>Priority</th>
    <th>Epic</th>
  </tr>
  <tr>
    <td>US16</td>
    <td>Supervisor de logistica</td>
    <td>Alta</td>
    <td>EP04 - Almacenamiento y Sincronizacion de Datos</td>
  </tr>

  <tr>
    <th>Title</th>
    <td colspan="3">Sincronizar datos con la nube automaticamente</td>
  </tr>

  <tr>
    <th colspan="4">Description</th>
  </tr>
  <tr>
    <td colspan="4">
      Como supervisor de logistica, quiero que los datos almacenados localmente se sincronicen automaticamente con la nube cuando haya conectividad disponible, para tener trazabilidad completa y respaldo de la informacion.
    </td>
  </tr>

  <tr>
    <th colspan="4">Acceptance Criteria</th>
  </tr>
  <tr>
    <td colspan="4">
      <p><strong>Escenario 01: Sincronizacion automatica al detectar WiFi</strong></p>
      <ul>
        <li>Dado que el contenedor regresa a una zona con conexion a internet,</li>
        <li>Cuando el sistema detecta una red WiFi configurada o datos moviles,</li>
        <li>Entonces inicia automaticamente la sincronizacion de datos pendientes con la nube,</li>
        <li>Y mantiene actualizado el historial centralizado.</li>
      </ul>
      <p><strong>Escenario 02: Resumen de sincronizacion</strong></p>
      <ul>
        <li>Dado que la sincronizacion ha finalizado,</li>
        <li>Cuando el supervisor revisa el dashboard,</li>
        <li>Entonces puede ver un resumen de los datos sincronizados y confirmar que no hubo perdida de informacion,</li>
        <li>Y valida la integridad del respaldo en nube.</li>
      </ul>
    </td>
  </tr>
</table>

<!-- US17 -->
<table border="1" cellspacing="0" cellpadding="8">
  <tr>
    <th>Story ID</th>
    <th>User</th>
    <th>Priority</th>
    <th>Epic</th>
  </tr>
  <tr>
    <td>US17</td>
    <td>Administrador de ONG</td>
    <td>Alta</td>
    <td>EP04 - Almacenamiento y Sincronizacion de Datos</td>
  </tr>

  <tr>
    <th>Title</th>
    <td colspan="3">Generar reporte de trazabilidad para donantes</td>
  </tr>

  <tr>
    <th colspan="4">Description</th>
  </tr>
  <tr>
    <td colspan="4">
      Como administrador de ONG, quiero generar un reporte de trazabilidad completo de un envio o proyecto, para presentar evidencia a donantes internacionales sobre el uso adecuado de los recursos.
    </td>
  </tr>

  <tr>
    <th colspan="4">Acceptance Criteria</th>
  </tr>
  <tr>
    <td colspan="4">
      <p><strong>Escenario 01: Generacion de reporte por envio</strong></p>
      <ul>
        <li>Dado que un envio ha sido completado y sincronizado,</li>
        <li>Cuando el administrador selecciona el envio y la opcion "Generar reporte",</li>
        <li>Entonces el sistema crea un documento PDF con graficos de temperatura, mapa de ruta, incidentes y estado final,</li>
        <li>Y deja evidencia formal para auditoria de donantes.</li>
      </ul>
      <p><strong>Escenario 02: Reporte consolidado por proyecto</strong></p>
      <ul>
        <li>Dado que un proyecto incluye multiples envios,</li>
        <li>Cuando el administrador selecciona el proyecto y un rango de fechas,</li>
        <li>Entonces el sistema genera un reporte consolidado con resumen de todos los envios y estadisticas agregadas,</li>
        <li>Y facilita la rendicion de cuentas del proyecto.</li>
      </ul>
    </td>
  </tr>
</table>

<!-- US18 -->
<table border="1" cellspacing="0" cellpadding="8">
  <tr>
    <th>Story ID</th>
    <th>User</th>
    <th>Priority</th>
    <th>Epic</th>
  </tr>
  <tr>
    <td>US18</td>
    <td>Administrador</td>
    <td>Media</td>
    <td>EP05 - Gestion de Usuarios y Roles</td>
  </tr>

  <tr>
    <th>Title</th>
    <td colspan="3">Ejecutar override manual mediante boton fisico</td>
  </tr>

  <tr>
    <th colspan="4">Description</th>
  </tr>
  <tr>
    <td colspan="4">
      Como operador autorizado, quiero ejecutar override manual mediante botones fisicos en el contenedor, para desbloquear la caja o silenciar alertas en situaciones de emergencia cuando no tengo acceso a la app.
    </td>
  </tr>

  <tr>
    <th colspan="4">Acceptance Criteria</th>
  </tr>
  <tr>
    <td colspan="4">
      <p><strong>Escenario 01: Desbloqueo por override fisico</strong></p>
      <ul>
        <li>Dado que el contenedor esta bloqueado por una condicion critica,</li>
        <li>Cuando el operador autorizado presiona el boton de override y ingresa su codigo,</li>
        <li>Entonces el servo desbloquea el contenedor y se registra la accion con el ID del operador,</li>
        <li>Y queda constancia para seguimiento posterior.</li>
      </ul>
      <p><strong>Escenario 02: Silenciar buzzer mediante boton fisico</strong></p>
      <ul>
        <li>Dado que el buzzer esta activo por una alerta,</li>
        <li>Cuando el operador presiona el boton de silencio,</li>
        <li>Entonces el buzzer se desactiva pero el LED rojo continua parpadeando,</li>
        <li>Y la alerta visual se mantiene hasta resolver la condicion.</li>
      </ul>
    </td>
  </tr>
</table>

<!-- US19 -->
<table border="1" cellspacing="0" cellpadding="8">
  <tr>
    <th>Story ID</th>
    <th>User</th>
    <th>Priority</th>
    <th>Epic</th>
  </tr>
  <tr>
    <td>US19</td>
    <td>Supervisor de logistica</td>
    <td>Media</td>
    <td>EP05 - Gestion de Usuarios y Roles</td>
  </tr>

  <tr>
    <th>Title</th>
    <td colspan="3">Ejecutar override remoto desde app o web</td>
  </tr>

  <tr>
    <th colspan="4">Description</th>
  </tr>
  <tr>
    <td colspan="4">
      Como supervisor de logistica, quiero ejecutar override remoto desde la app o web, para autorizar el desbloqueo del contenedor a distancia sin necesidad de que el operador este fisicamente presente.
    </td>
  </tr>

  <tr>
    <th colspan="4">Acceptance Criteria</th>
  </tr>
  <tr>
    <td colspan="4">
      <p><strong>Escenario 01: Override remoto por supervisor</strong></p>
      <ul>
        <li>Dado que el operador solicita autorizacion para abrir el contenedor en una zona remota,</li>
        <li>Cuando el supervisor recibe la solicitud en la app y la aprueba,</li>
        <li>Entonces el sistema envia una senal al contenedor para desbloquear el servo temporalmente,</li>
        <li>Y habilita la apertura bajo control remoto autorizado.</li>
      </ul>
      <p><strong>Escenario 02: Registro de override remoto</strong></p>
      <ul>
        <li>Dado que se ejecuto un override remoto,</li>
        <li>Cuando se revisa el log del envio,</li>
        <li>Entonces se registra quien autorizo, desde que dispositivo, en que momento y la duracion del desbloqueo,</li>
        <li>Y se conserva trazabilidad completa de la aprobacion.</li>
      </ul>
    </td>
  </tr>
</table>

<!-- US20 -->
<table border="1" cellspacing="0" cellpadding="8">
  <tr>
    <th>Story ID</th>
    <th>User</th>
    <th>Priority</th>
    <th>Epic</th>
  </tr>
  <tr>
    <td>US20</td>
    <td>Administrador</td>
    <td>Alta</td>
    <td>EP05 - Gestion de Usuarios y Roles</td>
  </tr>

  <tr>
    <th>Title</th>
    <td colspan="3">Configurar rangos permitidos por tipo de producto</td>
  </tr>

  <tr>
    <th colspan="4">Description</th>
  </tr>
  <tr>
    <td colspan="4">
      Como administrador, quiero configurar los rangos permitidos de temperatura, humedad y vibracion segun el tipo de producto (vacunas, insulina, sangre), para que el sistema evalue correctamente las condiciones segun los requerimientos especificos de cada producto.
    </td>
  </tr>

  <tr>
    <th colspan="4">Acceptance Criteria</th>
  </tr>
  <tr>
    <td colspan="4">
      <p><strong>Escenario 01: Seleccion de producto predefinido</strong></p>
      <ul>
        <li>Dado que el administrador esta configurando un nuevo envio,</li>
        <li>Cuando selecciona un tipo de producto de la lista predefinida (ej. Vacuna Pfizer, Insulina),</li>
        <li>Entonces el sistema carga automaticamente los rangos permitidos recomendados por el fabricante,</li>
        <li>Y aplica los parametros al envio configurado.</li>
      </ul>
      <p><strong>Escenario 02: Configuracion manual de rangos personalizados</strong></p>
      <ul>
        <li>Dado que el producto no esta en la lista predefinida,</li>
        <li>Cuando el administrador ingresa valores manuales para temperatura minima, maxima y otros parametros,</li>
        <li>Entonces el sistema guarda la configuracion y la aplica a todos los envios de ese producto,</li>
        <li>Y conserva la plantilla para futuras operaciones.</li>
      </ul>
    </td>
  </tr>
</table>

## **Technical Stories**
En esta sección se describen las historias técnicas que desarrollamos para implementar las funcionalidades clave. Cada historia define tareas específicas que el equipo de desarrollo debe realizar, como crear endpoints, supervisar el sistema, generar reportes, entre otros.

<!-- TS01 -->
<table border="1" cellspacing="0" cellpadding="8">
  <tr>
    <th>Story ID</th>
    <th>User</th>
    <th>Priority</th>
    <th>Epic</th>
  </tr>
  <tr>
    <td>TS01</td>
    <td>Developer</td>
    <td>Alta</td>
    <td>EP06 - Backend y API</td>
  </tr>
  <tr>
    <th>Title</th>
    <td colspan="3">API Sincronización de datos desde dispositivo IoT</td>
  </tr>
  <tr>
    <th colspan="4">Description</th>
  </tr>
  <tr>
    <td colspan="4">Como desarrollador, necesito exponer un endpoint para que el dispositivo CryoGuard sincronice los datos almacenados localmente (temperatura, humedad, vibración, GPS, eventos de apertura) con la nube cuando haya conectividad disponible, asegurando la integridad y trazabilidad de la información.</td>
  </tr>
  <tr>
    <th colspan="4">Acceptance Criteria</th>
  </tr>
  <tr>
    <td colspan="4">
      <p><strong>Escenario 01: Sincronización exitosa de datos</strong></p>
      <ul>
        <li>Dado que el dispositivo tiene datos pendientes en su almacenamiento local (tarjeta SD),</li>
        <li>Cuando detecta conexión a internet y envía los datos al endpoint de sincronización,</li>
        <li>Entonces el backend recibe, valida y almacena los datos en la base de datos,</li>
        <li>Y retorna código 201 con confirmación de recepción.</li>
      </ul>
      <p><strong>Escenario 02: Datos duplicados o ya sincronizados</strong></p>
      <ul>
        <li>Dado que el dispositivo envía un lote de datos ya sincronizados previamente,</li>
        <li>Cuando el endpoint recibe datos con IDs duplicados,</li>
        <li>Entonces el backend responde con código 200 indicando que ya existen,</li>
        <li>Y no duplica registros en la base de datos.</li>
      </ul>
      <p><strong>Escenario 03: Error de conexión durante sincronización</strong></p>
      <ul>
        <li>Dado que el dispositivo está enviando datos y la conexión se interrumpe,</li>
        <li>Cuando el endpoint no recibe el lote completo,</li>
        <li>Entonces el backend no almacena datos parciales,</li>
        <li>Y el dispositivo reintenta el envío completo en la siguiente sincronización.</li>
      </ul>
    </td>
  </tr>
</table>

<!-- TS02 -->
<table border="1" cellspacing="0" cellpadding="8">
  <tr>
    <th>Story ID</th>
    <th>User</th>
    <th>Priority</th>
    <th>Epic</th>
  </tr>
  <tr>
    <td>TS02</td>
    <td>Developer</td>
    <td>Alta</td>
    <td>EP06 - Backend y API</td>
  </tr>
  <tr>
    <th>Title</th>
    <td colspan="3">API Gestión de flags y alertas</td>
  </tr>
  <tr>
    <th colspan="4">Description</th>
  </tr>
  <tr>
    <td colspan="4">Como desarrollador, necesito exponer endpoints para que el dispositivo IoT envíe flags generados localmente (edge computing) y para que la web/app consulten alertas activas, permitiendo la supervisión en tiempo real de condiciones críticas.</td>
  </tr>
  <tr>
    <th colspan="4">Acceptance Criteria</th>
  </tr>
  <tr>
    <td colspan="4">
      <p><strong>Escenario 01: Recepción de flag crítico desde dispositivo</strong></p>
      <ul>
        <li>Dado que el dispositivo detecta una condición fuera de rango (ej. temperatura &gt; 8°C),</li>
        <li>Cuando envía el flag al endpoint correspondiente,</li>
        <li>Entonces el backend registra el flag con timestamp, tipo, valor y ubicación GPS,</li>
        <li>Y activa el proceso de notificaciones push a usuarios suscritos al envío.</li>
      </ul>
      <p><strong>Escenario 02: Consulta de flags activos por usuario</strong></p>
      <ul>
        <li>Dado que un supervisor accede al dashboard,</li>
        <li>Cuando consume el endpoint GET /flags?estado=activo,</li>
        <li>Entonces el backend retorna la lista de flags activos ordenados por prioridad,</li>
        <li>Y solo incluye envíos asociados al usuario (por región o rol).</li>
      </ul>
      <p><strong>Escenario 03: Confirmación de flag (override)</strong></p>
      <ul>
        <li>Dado que un usuario autorizado confirma un flag desde la app,</li>
        <li>Cuando consume el endpoint PUT /flags/{id}/confirmar,</li>
        <li>Entonces el backend actualiza el estado del flag a confirmado,</li>
        <li>Y registra quién lo confirmó, desde qué dispositivo y en qué momento.</li>
      </ul>
    </td>
  </tr>
</table>

<!-- TS03 -->
<table border="1" cellspacing="0" cellpadding="8">
  <tr>
    <th>Story ID</th>
    <th>User</th>
    <th>Priority</th>
    <th>Epic</th>
  </tr>
  <tr>
    <td>TS03</td>
    <td>Developer</td>
    <td>Alta</td>
    <td>EP06 - Backend y API</td>
  </tr>
  <tr>
    <th>Title</th>
    <td colspan="3">API Gestión de usuarios y roles</td>
  </tr>
  <tr>
    <th colspan="4">Description</th>
  </tr>
  <tr>
    <td colspan="4">Como desarrollador, necesito exponer endpoints para gestionar usuarios (crear, modificar, eliminar) y asignar roles (Operador, Supervisor, Administrador, ONG), asegurando autenticación segura y control de acceso basado en permisos.</td>
  </tr>
  <tr>
    <th colspan="4">Acceptance Criteria</th>
  </tr>
  <tr>
    <td colspan="4">
      <p><strong>Escenario 01: Registro exitoso de usuario</strong></p>
      <ul>
        <li>Dado que el administrador o el registro público está disponible,</li>
        <li>Cuando el usuario envía email, contraseña válida y datos básicos,</li>
        <li>Entonces el backend crea la cuenta en la base de datos y retorna token JWT o código 201,</li>
        <li>Y la contraseña se almacena hasheada (bcrypt/argon2).</li>
      </ul>
      <p><strong>Escenario 02: Registro con email duplicado o datos inválidos</strong></p>
      <ul>
        <li>Dado que el endpoint de registro recibe datos,</li>
        <li>Cuando el email ya existe o la contraseña no cumple requisitos,</li>
        <li>Entonces el backend responde con código 409 (duplicado) o 400 (validación),</li>
        <li>Y retorna un mensaje claro con el error específico.</li>
      </ul>
      <p><strong>Escenario 03: Autenticación de usuario (login)</strong></p>
      <ul>
        <li>Dado que un usuario tiene una cuenta activa,</li>
        <li>Cuando envía sus credenciales al endpoint /auth/login,</li>
        <li>Entonces el backend valida credenciales y retorna JWT con expiración configurada,</li>
        <li>Y el rol/permisos del usuario quedan codificados en el token.</li>
      </ul>
      <p><strong>Escenario 04: Asignación de rol por administrador</strong></p>
      <ul>
        <li>Dado que un administrador gestiona usuarios desde el dashboard,</li>
        <li>Cuando asigna o modifica el rol de un usuario,</li>
        <li>Entonces el backend actualiza permisos del usuario,</li>
        <li>Y registra la acción en un log de auditoría.</li>
      </ul>
    </td>
  </tr>
</table>

<!-- TS04 -->
<table border="1" cellspacing="0" cellpadding="8">
  <tr>
    <th>Story ID</th>
    <th>User</th>
    <th>Priority</th>
    <th>Epic</th>
  </tr>
  <tr>
    <td>TS04</td>
    <td>Developer</td>
    <td>Media</td>
    <td>EP06 - Backend y API</td>
  </tr>
  <tr>
    <th>Title</th>
    <td colspan="3">API Generación de reportes de trazabilidad</td>
  </tr>
  <tr>
    <th colspan="4">Description</th>
  </tr>
  <tr>
    <td colspan="4">Como desarrollador, necesito exponer endpoints para generar reportes de trazabilidad (por envío, por proyecto o por rango de fechas) en formatos PDF y Excel, para que supervisores y ONGs presenten evidencia a donantes y entes reguladores.</td>
  </tr>
  <tr>
    <th colspan="4">Acceptance Criteria</th>
  </tr>
  <tr>
    <td colspan="4">
      <p><strong>Escenario 01: Generación de reporte por ID de envío</strong></p>
      <ul>
        <li>Dado que un supervisor selecciona un envío completado,</li>
        <li>Cuando consume GET /reportes/envio/{id}?formato=pdf,</li>
        <li>Entonces el backend genera un PDF con gráficos, mapa de ruta, incidentes y estado final,</li>
        <li>Y retorna el archivo para descarga.</li>
      </ul>
      <p><strong>Escenario 02: Generación de reporte consolidado por proyecto</strong></p>
      <ul>
        <li>Dado que una ONG necesita reportar múltiples envíos de un proyecto,</li>
        <li>Cuando consume POST /reportes/proyecto con rango de fechas y lista de envíos,</li>
        <li>Entonces el backend genera un consolidado con resumen estadístico y porcentaje de éxito,</li>
        <li>Y retorna el archivo en formato PDF o Excel.</li>
      </ul>
      <p><strong>Escenario 03: Cache de reportes para evitar regeneración</strong></p>
      <ul>
        <li>Dado que el mismo reporte se solicita múltiples veces sin cambios de datos,</li>
        <li>Cuando el backend recibe una solicitud idéntica (mismos parámetros),</li>
        <li>Entonces retorna el reporte en caché sin regenerar documento,</li>
        <li>Y reduce tiempo de respuesta y carga del servidor.</li>
      </ul>
    </td>
  </tr>
</table>

<!-- TS05 -->
<table border="1" cellspacing="0" cellpadding="8">
  <tr>
    <th>Story ID</th>
    <th>User</th>
    <th>Priority</th>
    <th>Epic</th>
  </tr>
  <tr>
    <td>TS05</td>
    <td>Embedded Developer</td>
    <td>Alta</td>
    <td>EP07 - Dispositivo IoT y Edge Computing</td>
  </tr>
  <tr>
    <th>Title</th>
    <td colspan="3">Implementar lectura de sensores (temp, humedad, vibración, GPS, apertura)</td>
  </tr>
  <tr>
    <th colspan="4">Description</th>
  </tr>
  <tr>
    <td colspan="4">Como desarrollador embedded, necesito implementar la lectura de todos los sensores del dispositivo CryoGuard, asegurando captura de datos en intervalos configurables y almacenamiento local en tarjeta SD.</td>
  </tr>
  <tr>
    <th colspan="4">Acceptance Criteria</th>
  </tr>
  <tr>
    <td colspan="4">
      <p><strong>Escenario 01: Lectura periódica de sensores</strong></p>
      <ul>
        <li>Dado que el dispositivo está encendido y en modo operación,</li>
        <li>Cuando el temporizador alcanza el intervalo configurado (ej. cada 30 segundos),</li>
        <li>Entonces el sistema lee todos los sensores,</li>
        <li>Y almacena datos en tarjeta SD con timestamp y GPS actual.</li>
      </ul>
      <p><strong>Escenario 02: Almacenamiento local en tarjeta SD</strong></p>
      <ul>
        <li>Dado que el dispositivo está en zona sin conectividad,</li>
        <li>Cuando los sensores capturan datos,</li>
        <li>Entonces los datos se escriben en la tarjeta SD en formato CSV o JSON,</li>
        <li>Y se mantienen hasta la siguiente sincronización exitosa.</li>
      </ul>
      <p><strong>Escenario 03: Detección de fallo de sensor</strong></p>
      <ul>
        <li>Dado que un sensor no responde o envía datos inválidos,</li>
        <li>Cuando el sistema intenta leerlo,</li>
        <li>Entonces registra un error interno y continúa con los sensores restantes,</li>
        <li>Y genera un flag de mantenimiento para el supervisor.</li>
      </ul>
    </td>
  </tr>
</table>

<!-- TS06 -->
<table border="1" cellspacing="0" cellpadding="8">
  <tr>
    <th>Story ID</th>
    <th>User</th>
    <th>Priority</th>
    <th>Epic</th>
  </tr>
  <tr>
    <td>TS06</td>
    <td>Embedded Developer</td>
    <td>Alta</td>
    <td>EP07 - Dispositivo IoT y Edge Computing</td>
  </tr>
  <tr>
    <th>Title</th>
    <td colspan="3">Implementar reglas de edge computing para generación de flags</td>
  </tr>
  <tr>
    <th colspan="4">Description</th>
  </tr>
  <tr>
    <td colspan="4">Como desarrollador embedded, necesito implementar un motor de reglas que evalúe localmente los datos de sensores y genere flags preventivos o críticos cuando las variables salgan de rango, activando actuadores automáticamente.</td>
  </tr>
  <tr>
    <th colspan="4">Acceptance Criteria</th>
  </tr>
  <tr>
    <td colspan="4">
      <p><strong>Escenario 01: Evaluación de temperatura fuera de rango</strong></p>
      <ul>
        <li>Dado que el rango permitido es 2°C a 8°C,</li>
        <li>Cuando el sensor registra 9°C durante más de 30 segundos,</li>
        <li>Entonces el sistema genera un flag crítico,</li>
        <li>Y activa LED rojo, buzzer y Peltier automáticamente.</li>
      </ul>
      <p><strong>Escenario 02: Evaluación de temperatura cercana al límite</strong></p>
      <ul>
        <li>Dado que el rango permitido es 2°C a 8°C,</li>
        <li>Cuando el sensor registra 7.5°C cercano al límite superior,</li>
        <li>Entonces el sistema genera un flag preventivo,</li>
        <li>Y activa LED amarillo sin buzzer.</li>
      </ul>
      <p><strong>Escenario 03: Evaluación de vibración excesiva</strong></p>
      <ul>
        <li>Dado que existe un umbral máximo de vibración configurado,</li>
        <li>Cuando el sensor registra un valor superior al umbral,</li>
        <li>Entonces el sistema genera un flag de vibración,</li>
        <li>Y registra el evento sin activar enfriamiento.</li>
      </ul>
      <p><strong>Escenario 04: Evaluación de apertura no autorizada</strong></p>
      <ul>
        <li>Dado que el contenedor está cerrado y no hay override activo,</li>
        <li>Cuando el sensor de apertura detecta que la caja se abrió,</li>
        <li>Entonces el sistema genera un flag crítico de apertura no autorizada,</li>
        <li>Y activa LED rojo, buzzer y bloqueo de servo.</li>
      </ul>
    </td>
  </tr>
</table>

<!-- TS07 -->
<table border="1" cellspacing="0" cellpadding="8">
  <tr>
    <th>Story ID</th>
    <th>User</th>
    <th>Priority</th>
    <th>Epic</th>
  </tr>
  <tr>
    <td>TS07</td>
    <td>Embedded Developer</td>
    <td>Alta</td>
    <td>EP07 - Dispositivo IoT y Edge Computing</td>
  </tr>
  <tr>
    <th>Title</th>
    <td colspan="3">Implementar control de actuadores (Peltier, Servo, LED, Buzzer)</td>
  </tr>
  <tr>
    <th colspan="4">Description</th>
  </tr>
  <tr>
    <td colspan="4">Como desarrollador embedded, necesito implementar el control de actuadores del dispositivo por reglas automáticas y por comandos manuales (botones físicos o remotos).</td>
  </tr>
  <tr>
    <th colspan="4">Acceptance Criteria</th>
  </tr>
  <tr>
    <td colspan="4">
      <p><strong>Escenario 01: Activación automática de Peltier por temperatura alta</strong></p>
      <ul>
        <li>Dado que se detectó un flag crítico por temperatura alta,</li>
        <li>Cuando el sistema evalúa la regla correspondiente,</li>
        <li>Entonces activa módulo Peltier, disipador y ventilador,</li>
        <li>Y mantiene enfriamiento hasta normalización sostenida por 2 minutos.</li>
      </ul>
      <p><strong>Escenario 02: Activación de servo para bloqueo de apertura</strong></p>
      <ul>
        <li>Dado que se detectó un flag crítico o apertura no autorizada,</li>
        <li>Cuando el sistema activa el bloqueo,</li>
        <li>Entonces el servo bloquea físicamente la apertura del contenedor,</li>
        <li>Y solo se desbloquea con override autorizado.</li>
      </ul>
      <p><strong>Escenario 03: Control de LEDs según estado</strong></p>
      <ul>
        <li>Dado que no hay flags activos, cuando se evalúa estado normal, entonces LED verde fijo.</li>
        <li>Dado que hay flag preventivo activo, cuando la condición es cercana al límite, entonces LED amarillo fijo.</li>
        <li>Dado que hay flag crítico activo, cuando la condición está fuera de rango, entonces LED rojo parpadeante.</li>
        <li>Y el patrón visual refleja de forma inmediata la severidad actual.</li>
      </ul>
      <p><strong>Escenario 04: Control de buzzer para alertas sonoras</strong></p>
      <ul>
        <li>Dado que hay un flag crítico activo,</li>
        <li>Cuando se activa la alerta sonora,</li>
        <li>Entonces el buzzer emite pitido intermitente y puede silenciarse por botón físico,</li>
        <li>Pero el LED rojo continúa parpadeando hasta normalizar la condición.</li>
      </ul>
    </td>
  </tr>
</table>

<!-- TS08 -->
<table border="1" cellspacing="0" cellpadding="8">
  <tr>
    <th>Story ID</th>
    <th>User</th>
    <th>Priority</th>
    <th>Epic</th>
  </tr>
  <tr>
    <td>TS08</td>
    <td>Embedded Developer</td>
    <td>Media</td>
    <td>EP07 - Dispositivo IoT y Edge Computing</td>
  </tr>
  <tr>
    <th>Title</th>
    <td colspan="3">Implementar botones físicos para override y control manual</td>
  </tr>
  <tr>
    <th colspan="4">Description</th>
  </tr>
  <tr>
    <td colspan="4">Como desarrollador embedded, necesito implementar lectura de botones físicos (override, silencio, prueba de LEDs, reset) para permitir acciones manuales sin depender de app o web.</td>
  </tr>
  <tr>
    <th colspan="4">Acceptance Criteria</th>
  </tr>
  <tr>
    <td colspan="4">
      <p><strong>Escenario 01: Override manual mediante botón físico</strong></p>
      <ul>
        <li>Dado que el contenedor está bloqueado por un flag crítico,</li>
        <li>Cuando el operador autorizado presiona el botón de override por 3 segundos,</li>
        <li>Entonces el sistema desbloquea el servo por 30 segundos,</li>
        <li>Y registra la acción en el log con timestamp e identificador.</li>
      </ul>
      <p><strong>Escenario 02: Silencio de buzzer mediante botón físico</strong></p>
      <ul>
        <li>Dado que el buzzer está activo por un flag crítico,</li>
        <li>Cuando el operador presiona el botón de silencio,</li>
        <li>Entonces el buzzer se desactiva inmediatamente,</li>
        <li>Pero el LED rojo continúa parpadeando hasta normalizar la condición.</li>
      </ul>
      <p><strong>Escenario 03: Prueba de LEDs y buzzer</strong></p>
      <ul>
        <li>Dado que el operador quiere verificar actuadores,</li>
        <li>Cuando presiona el botón de prueba,</li>
        <li>Entonces el sistema enciende LED rojo, amarillo y verde en secuencia,</li>
        <li>Y activa el buzzer por 1 segundo.</li>
      </ul>
    </td>
  </tr>
</table>

<!-- TS09 -->
<table border="1" cellspacing="0" cellpadding="8">
  <tr>
    <th>Story ID</th>
    <th>User</th>
    <th>Priority</th>
    <th>Epic</th>
  </tr>
  <tr>
    <td>TS09</td>
    <td>Frontend Developer</td>
    <td>Alta</td>
    <td>EP08 - Dashboard Web</td>
  </tr>
  <tr>
    <th>Title</th>
    <td colspan="3">Implementar dashboard con mapa interactivo de envíos activos</td>
  </tr>
  <tr>
    <th colspan="4">Description</th>
  </tr>
  <tr>
    <td colspan="4">Como desarrollador frontend, necesito implementar un dashboard web con mapa interactivo para visualizar contenedores activos y su estado en tiempo real.</td>
  </tr>
  <tr>
    <th colspan="4">Acceptance Criteria</th>
  </tr>
  <tr>
    <td colspan="4">
      <p><strong>Escenario 01: Carga inicial del mapa con envíos activos</strong></p>
      <ul>
        <li>Dado que un supervisor autenticado accede al dashboard,</li>
        <li>Cuando la página se carga,</li>
        <li>Entonces el frontend consume GET /envios/activos y renderiza marcadores activos,</li>
        <li>Y cada marcador muestra color según estado del envío.</li>
      </ul>
      <p><strong>Escenario 02: Actualización en tiempo real de posiciones</strong></p>
      <ul>
        <li>Dado que el dashboard está abierto y hay envíos en movimiento,</li>
        <li>Cuando el backend recibe nuevos datos de ubicación,</li>
        <li>Entonces el frontend actualiza posiciones sin recargar la página,</li>
        <li>Mediante WebSockets o polling cada 10 segundos.</li>
      </ul>
      <p><strong>Escenario 03: Click en marcador para ver detalles del envío</strong></p>
      <ul>
        <li>Dado que el supervisor hace click en un marcador,</li>
        <li>Cuando se abre un panel lateral,</li>
        <li>Entonces muestra ID, producto, temperatura actual, flags activos y último dato de humedad,</li>
        <li>Y permite supervisión operativa contextual por envío.</li>
      </ul>
    </td>
  </tr>
</table>

<!-- TS10 -->
<table border="1" cellspacing="0" cellpadding="8">
  <tr>
    <th>Story ID</th>
    <th>User</th>
    <th>Priority</th>
    <th>Epic</th>
  </tr>
  <tr>
    <td>TS10</td>
    <td>Frontend Developer</td>
    <td>Alta</td>
    <td>EP08 - Dashboard Web</td>
  </tr>
  <tr>
    <th>Title</th>
    <td colspan="3">Implementar tabla de logs históricos con filtros y exportación</td>
  </tr>
  <tr>
    <th colspan="4">Description</th>
  </tr>
  <tr>
    <td colspan="4">Como desarrollador frontend, necesito implementar tabla paginada de logs históricos con filtros por fecha/región/producto/estado y exportación a CSV/PDF.</td>
  </tr>
  <tr>
    <th colspan="4">Acceptance Criteria</th>
  </tr>
  <tr>
    <td colspan="4">
      <p><strong>Escenario 01: Visualización de tabla de logs</strong></p>
      <ul>
        <li>Dado que un supervisor accede a la sección de historial,</li>
        <li>Cuando la página se carga,</li>
        <li>Entonces el frontend consume GET /logs?page=1&amp;limit=50 y renderiza tabla de resultados,</li>
        <li>Y muestra columnas de envío, fecha, producto, promedio, incidentes y estado final.</li>
      </ul>
      <p><strong>Escenario 02: Filtros combinados</strong></p>
      <ul>
        <li>Dado que el supervisor aplica filtros combinados,</li>
        <li>Cuando hace click en Aplicar filtros,</li>
        <li>Entonces el frontend consume endpoint con parámetros de filtro,</li>
        <li>Y actualiza la tabla con resultados filtrados.</li>
      </ul>
      <p><strong>Escenario 03: Exportación a CSV/PDF</strong></p>
      <ul>
        <li>Dado que el supervisor necesita exportar los logs filtrados,</li>
        <li>Cuando hace click en Exportar y selecciona CSV,</li>
        <li>Entonces el frontend descarga archivo con los datos de la tabla actual,</li>
        <li>Y respeta filtros aplicados en la exportación.</li>
      </ul>
    </td>
  </tr>
</table>

<!-- TS11 -->
<table border="1" cellspacing="0" cellpadding="8">
  <tr>
    <th>Story ID</th>
    <th>User</th>
    <th>Priority</th>
    <th>Epic</th>
  </tr>
  <tr>
    <td>TS11</td>
    <td>Frontend Developer</td>
    <td>Media</td>
    <td>EP08 - Dashboard Web</td>
  </tr>
  <tr>
    <th>Title</th>
    <td colspan="3">Implementar panel de administración de usuarios y roles</td>
  </tr>
  <tr>
    <th colspan="4">Description</th>
  </tr>
  <tr>
    <td colspan="4">Como desarrollador frontend, necesito implementar un panel para crear, modificar, eliminar usuarios y asignar roles (Operador, Supervisor, Administrador, ONG).</td>
  </tr>
  <tr>
    <th colspan="4">Acceptance Criteria</th>
  </tr>
  <tr>
    <td colspan="4">
      <p><strong>Escenario 01: Listado de usuarios con paginación</strong></p>
      <ul>
        <li>Dado que un administrador accede al panel de usuarios,</li>
        <li>Cuando la página se carga,</li>
        <li>Entonces el frontend consume GET /admin/usuarios y renderiza la tabla,</li>
        <li>Y muestra nombre, email, rol, fecha y estado.</li>
      </ul>
      <p><strong>Escenario 02: Creación de nuevo usuario</strong></p>
      <ul>
        <li>Dado que el administrador hace click en Nuevo usuario,</li>
        <li>Cuando completa formulario y confirma,</li>
        <li>Entonces el frontend envía POST /admin/usuarios,</li>
        <li>Y actualiza la tabla con el nuevo registro.</li>
      </ul>
      <p><strong>Escenario 03: Edición y eliminación de usuarios</strong></p>
      <ul>
        <li>Dado que el administrador selecciona un usuario de la tabla,</li>
        <li>Cuando edita rol o deshabilita cuenta,</li>
        <li>Entonces el frontend envía PUT o DELETE según corresponda,</li>
        <li>Y refresca la tabla reflejando los cambios.</li>
      </ul>
    </td>
  </tr>
</table>

<!-- TS12 -->
<table border="1" cellspacing="0" cellpadding="8">
  <tr>
    <th>Story ID</th>
    <th>User</th>
    <th>Priority</th>
    <th>Epic</th>
  </tr>
  <tr>
    <td>TS12</td>
    <td>Mobile Developer</td>
    <td>Alta</td>
    <td>EP09 - Aplicación Móvil</td>
  </tr>
  <tr>
    <th>Title</th>
    <td colspan="3">Implementar autenticación y pantalla de inicio en app móvil</td>
  </tr>
  <tr>
    <th colspan="4">Description</th>
  </tr>
  <tr>
    <td colspan="4">Como desarrollador móvil (iOS/Android), necesito implementar login/registro y pantalla de inicio para que operadores y supervisores accedan y vean sus envíos asignados.</td>
  </tr>
  <tr>
    <th colspan="4">Acceptance Criteria</th>
  </tr>
  <tr>
    <td colspan="4">
      <p><strong>Escenario 01: Login con email y contraseña</strong></p>
      <ul>
        <li>Dado que el usuario tiene una cuenta activa,</li>
        <li>Cuando ingresa credenciales y presiona Iniciar sesión,</li>
        <li>Entonces la app consume POST /auth/login y almacena JWT de forma segura,</li>
        <li>Y navega a la pantalla de inicio.</li>
      </ul>
      <p><strong>Escenario 02: Almacenamiento seguro de token</strong></p>
      <ul>
        <li>Dado que el usuario cierra y abre nuevamente la app,</li>
        <li>Cuando el token aún no ha expirado,</li>
        <li>Entonces la app restaura sesión automáticamente,</li>
        <li>Y evita solicitar login nuevamente.</li>
      </ul>
      <p><strong>Escenario 03: Pantalla de inicio con resumen de envíos</strong></p>
      <ul>
        <li>Dado que el usuario está autenticado y tiene envíos asignados,</li>
        <li>Cuando la app carga la pantalla de inicio,</li>
        <li>Entonces consume GET /envios/asignados y muestra lista de envíos activos,</li>
        <li>Y presenta ID, destino, temperatura y estado.</li>
      </ul>
    </td>
  </tr>
</table>

<!-- TS13 -->
<table border="1" cellspacing="0" cellpadding="8">
  <tr>
    <th>Story ID</th>
    <th>User</th>
    <th>Priority</th>
    <th>Epic</th>
  </tr>
  <tr>
    <td>TS13</td>
    <td>Mobile Developer</td>
    <td>Alta</td>
    <td>EP09 - Aplicación Móvil</td>
  </tr>
  <tr>
    <th>Title</th>
    <td colspan="3">Implementar recepción de notificaciones push</td>
  </tr>
  <tr>
    <th colspan="4">Description</th>
  </tr>
  <tr>
    <td colspan="4">Como desarrollador móvil, necesito implementar recepción de notificaciones push (FCM/APNs) para alertas en tiempo real por flags críticos de envíos asignados.</td>
  </tr>
  <tr>
    <th colspan="4">Acceptance Criteria</th>
  </tr>
  <tr>
    <td colspan="4">
      <p><strong>Escenario 01: Registro del dispositivo para notificaciones push</strong></p>
      <ul>
        <li>Dado que el usuario inicia sesión por primera vez,</li>
        <li>Cuando la app solicita permisos y el usuario los acepta,</li>
        <li>Entonces la app obtiene el token push y lo envía al backend,</li>
        <li>Y queda asociado al usuario autenticado.</li>
      </ul>
      <p><strong>Escenario 02: Recepción de notificación por flag crítico</strong></p>
      <ul>
        <li>Dado que el usuario tiene sesión activa o app en segundo plano,</li>
        <li>Cuando backend envía notificación por flag crítico asignado,</li>
        <li>Entonces la app muestra notificación en el centro del dispositivo,</li>
        <li>Y al tocarla abre detalle del envío.</li>
      </ul>
      <p><strong>Escenario 03: Contenido de la notificación</strong></p>
      <ul>
        <li>Dado que el usuario recibe una notificación push,</li>
        <li>Cuando la visualiza,</li>
        <li>Entonces el título indica Alerta CryoGuard - Flag Crítico,</li>
        <li>Y el cuerpo muestra tipo de flag, valor e ID de envío.</li>
      </ul>
    </td>
  </tr>
</table>

<!-- TS14 -->
<table border="1" cellspacing="0" cellpadding="8">
  <tr>
    <th>Story ID</th>
    <th>User</th>
    <th>Priority</th>
    <th>Epic</th>
  </tr>
  <tr>
    <td>TS14</td>
    <td>Mobile Developer</td>
    <td>Media</td>
    <td>EP09 - Aplicación Móvil</td>
  </tr>
  <tr>
    <th>Title</th>
    <td colspan="3">Implementar override remoto desde app móvil</td>
  </tr>
  <tr>
    <th colspan="4">Description</th>
  </tr>
  <tr>
    <td colspan="4">Como desarrollador móvil, necesito implementar override remoto para que supervisores autorizados desbloqueen contenedor a distancia o gestionen alertas cuando lo solicite el operador.</td>
  </tr>
  <tr>
    <th colspan="4">Acceptance Criteria</th>
  </tr>
  <tr>
    <td colspan="4">
      <p><strong>Escenario 01: Solicitud de override por operador</strong></p>
      <ul>
        <li>Dado que el contenedor está bloqueado y el operador necesita abrirlo,</li>
        <li>Cuando el operador solicita autorización desde app o por comunicación externa,</li>
        <li>Entonces el supervisor recibe una notificación push con la solicitud,</li>
        <li>Y puede revisar contexto del envío antes de aprobar.</li>
      </ul>
      <p><strong>Escenario 02: Aprobación de override por supervisor</strong></p>
      <ul>
        <li>Dado que el supervisor recibe la solicitud de override,</li>
        <li>Cuando abre la app, selecciona envío y presiona Autorizar desbloqueo,</li>
        <li>Entonces la app consume POST /envios/{id}/override-remoto y backend envía comando al IoT,</li>
        <li>Y registra la acción en el log con ID del supervisor.</li>
      </ul>
      <p><strong>Escenario 03: Confirmación de override exitoso</strong></p>
      <ul>
        <li>Dado que el comando de override fue enviado exitosamente,</li>
        <li>Cuando el dispositivo confirma la recepción,</li>
        <li>Entonces la app muestra mensaje Contenedor desbloqueado temporalmente,</li>
        <li>Y el operador puede abrir la caja.</li>
      </ul>
    </td>
  </tr>
</table>


## 3.2. Impact Mapping

El siguiente mapa de impacto conecta el objetivo de negocio con actores, impactos deseados y entregables del producto.

**Segmento #1: Centros de salud rurales o urbanos**
<img src="assets/Chapter-3/Impact map CryoGuard (1).png" alt="Impact Mapping - segmento 1" width="600"/>

_Imagen (N°8). Elaboración propia. Realizado en UXPressia_

**Segmento #2: ONGs y gestores de logística sanitaria (ej. UNICEF, MINSA, OPS, Cruz Roja)**
<img src="assets/Chapter-3/Impact map CryoGuard (2).png" alt="Impact Mapping - segmento 2" width="600"/>

_Imagen (N°9). Elaboración propia. Realizado en UXPressia_
<br> <!-- Esto agrega espacio visual en algunas plataformas -->
  
## 3.3. Product Backlog

Backlog inicial priorizado para la implementación incremental de CryoGuard.

<table border="1" cellspacing="0" cellpadding="8">
  <tr>
    <th>Prioridad</th>
    <th>User Story ID</th>
    <th>Título</th>
    <th>Story Points</th>
  </tr>
  <tr><td>1</td><td>US01</td><td>Monitorear temperatura en tiempo real</td><td>5</td></tr>
  <tr><td>2</td><td>US04</td><td>Geolocalizar contenedor en tiempo real</td><td>5</td></tr>
  <tr><td>3</td><td>US05</td><td>Activar enfriamiento automático (Peltier)</td><td>5</td></tr>
  <tr><td>4</td><td>US07</td><td>Recibir alerta visual mediante LED</td><td>5</td></tr>
  <tr><td>5</td><td>US08</td><td>Recibir alerta sonora mediante Buzzer</td><td>5</td></tr>
  <tr><td>6</td><td>US15</td><td>Almacenar datos localmente durante transporte offline</td><td>5</td></tr>
  <tr><td>7</td><td>TS01</td><td>API Sincronización de datos desde dispositivo IoT</td><td>5</td></tr>
  <tr><td>8</td><td>TS05</td><td>Implementar lectura de sensores (temp, humedad, vibración, GPS, apertura)</td><td>5</td></tr>
  <tr><td>9</td><td>TS06</td><td>Implementar reglas de edge computing para generación de flags</td><td>5</td></tr>
  <tr><td>10</td><td>TS07</td><td>Implementar control de actuadores (Peltier, Servo, LED, Buzzer)</td><td>5</td></tr>
  <tr><td>11</td><td>US02</td><td>Monitorear humedad del contenedor</td><td>4</td></tr>
  <tr><td>12</td><td>US10</td><td>Detectar apertura no autorizada del contenedor</td><td>4</td></tr>
  <tr><td>13</td><td>US11</td><td>Visualizar dashboard con mapa de envíos activos</td><td>4</td></tr>
  <tr><td>14</td><td>US13</td><td>Recibir notificaciones push en app móvil</td><td>4</td></tr>
  <tr><td>15</td><td>US16</td><td>Sincronizar datos con la nube automáticamente</td><td>4</td></tr>
  <tr><td>16</td><td>US20</td><td>Configurar rangos permitidos por tipo de producto</td><td>4</td></tr>
  <tr><td>17</td><td>TS02</td><td>API Gestión de flags y alertas</td><td>4</td></tr>
  <tr><td>18</td><td>TS03</td><td>API Gestión de usuarios y roles</td><td>4</td></tr>
  <tr><td>19</td><td>TS09</td><td>Implementar dashboard con mapa interactivo de envíos activos</td><td>4</td></tr>
  <tr><td>20</td><td>TS12</td><td>Implementar autenticación y pantalla de inicio en app móvil</td><td>4</td></tr>
  <tr><td>21</td><td>US03</td><td>Detectar vibraciones o impactos</td><td>3</td></tr>
  <tr><td>22</td><td>US06</td><td>Bloquear apertura del contenedor (Servo)</td><td>3</td></tr>
  <tr><td>23</td><td>US09</td><td>Detectar salida de geocerca</td><td>3</td></tr>
  <tr><td>24</td><td>US12</td><td>Consultar logs históricos de envíos</td><td>3</td></tr>
  <tr><td>25</td><td>US17</td><td>Generar reporte de trazabilidad para donantes</td><td>3</td></tr>
  <tr><td>26</td><td>US18</td><td>Ejecutar override manual mediante botón físico</td><td>3</td></tr>
  <tr><td>27</td><td>TS04</td><td>API Generación de reportes de trazabilidad</td><td>3</td></tr>
  <tr><td>28</td><td>TS08</td><td>Implementar botones físicos para override y control manual</td><td>3</td></tr>
  <tr><td>29</td><td>TS10</td><td>Implementar tabla de logs históricos con filtros y exportación</td><td>3</td></tr>
  <tr><td>30</td><td>TS13</td><td>Implementar recepción de notificaciones push</td><td>3</td></tr>
  <tr><td>31</td><td>US14</td><td>Gestionar usuarios y roles desde dashboard</td><td>2</td></tr>
  <tr><td>32</td><td>US19</td><td>Ejecutar override remoto desde app o web</td><td>2</td></tr>
  <tr><td>33</td><td>TS11</td><td>Implementar panel de administración de usuarios y roles</td><td>2</td></tr>
  <tr><td>34</td><td>TS14</td><td>Implementar override remoto desde app móvil</td><td>2</td></tr>
</table>

</div>
