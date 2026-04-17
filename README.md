# Capítulo III: Requirements Specification

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
  </tr>

  <tr>
    <th colspan="4">Description</th>
  </tr>
  <tr>
    <td colspan="4">
      Como supervisor de logistica, quiero recibir una alerta cuando el contenedor salga de la ruta o geocerca definida, para identificar desviaciones no planificadas.
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
  </tr>

  <tr>
    <th colspan="4">Description</th>
  </tr>
  <tr>
    <td colspan="4">
      Como supervisor de logistica, quiero recibir una alerta cuando el contenedor se abra sin autorizacion, para identificar posibles manipulaciones indebidas de los productos.
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

</div>
