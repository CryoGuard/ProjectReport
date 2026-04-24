## 4.1 Strategic-Level Domain-Driven Design.

### 4.1.1 Design-Level EventStorming.

Para comprender el comportamiento del sistema, se aplicó la técnica de Event Storming a nivel de diseño, identificando los principales eventos del dominio en distintos escenarios críticos del negocio.

Estos eventos representan situaciones relevantes que pueden ocurrir durante el monitoreo y transporte de los contenedores, permitiendo visualizar cómo reacciona el sistema ante cada caso.

Los escenarios analizados incluyen condiciones anómalas como temperatura fuera de rango, apertura no autorizada del contenedor, desvío de ruta, pérdida de conexión a internet y sincronización de datos.

<p align="center">
  <img src="assets/Chapter-4/eventstorming5.png" width="650"/>
</p>

<p align="center">
  <img src="assets/Chapter-4/eventstorming0.png" width="650"/>
</p>

<p align="center">
  <img src="assets/Chapter-4//eventstorming1.png" width="650"/>
</p>

<p align="center">
  <img src="assets/Chapter-4/eventstorming2.png" width="650"/>
</p>

<p align="center">
  <img src="assets/Chapter-4/eventstorming3.png" width="650"/>
</p>

<p align="center">
  <img src="assets/Chapter-4/eventstorming4.png" width="650"/>
</p>

### 4.1.1.1 Candidate Context Discovery.

A partir de los eventos identificados en el Event Storming, se analizaron agrupaciones naturales según la responsabilidad funcional dentro del sistema.

Este análisis permitió relacionar cada escenario con los Bounded Contexts previamente definidos por el equipo, asegurando coherencia entre el modelado del dominio y la arquitectura propuesta.

Los eventos fueron alineados con los siguientes Bounded Contexts existentes:

<p align="center">
  <img src="assets/Chapter-4/CandidateContextDiscovery.png" width="650"/>
</p>

### 4.1.1.2 Domain Message Flows Modeling.

En esta sección, se modeló la colaboración entre los Bounded Contexts para resolver los casos de uso críticos de CryoGuard. Se utilizó la técnica de Domain Storytelling, que permite visualizar la narrativa del negocio mediante el intercambio de mensajes entre actores, sistemas y contextos.


<p align="center">
  <img src="assets/Chapter-4/flowsModeling1.jpg" width="650"/>
</p>

El Sensor IoT detecta una temperatura fuera de los parámetros permitidos y envía el mensaje a Evaluation Management. Este contexto genera la alerta hacia IoT Monitoring Management, la cual viaja a través de la CryoGuard Platform. Finalmente, Operations Management procesa la información para que el Operador Logístico visualice la alerta y tome medidas.

<p align="center">
  <img src="assets/Chapter-4/flowsModeling2.jpg" width="650"/>
</p>

Al detectar una desviación, el Sensor IoT lo comunica a Logistics Management, que genera una alerta de ubicación. El mensaje pasa por IoT Monitoring Management hacia la CryoGuard Platform. Desde allí, Operations Management registra el desvío, permitiendo que el Operador Logístico visualice la ruta y la alerta en su pantalla.

<p align="center">
  <img src="assets/Chapter-4/flowsModeling3.jpg" width="650"/>
</p>

El Sensor IoT detecta la apertura física y IAM Management valida que no cuenta con autorización. Se genera una alerta de seguridad hacia IoT Monitoring Management que llega a la CryoGuard Platform. El sistema envía la notificación a Operations Management para almacenar el incidente y el Operador Logístico recibe la alerta de seguridad inmediata.

<p align="center">
  <img src="assets/Chapter-4/flowsModeling4.jpg" width="650"/>
</p>

El Sensor IoT verifica la conexión y IoT Monitoring Management detecta la pérdida de red. Ante esto, Operations Management activa el almacenamiento local para no perder datos. La información se registra temporalmente en el dispositivo y la CryoGuard Platform reporta al Operador Logístico la falta de monitoreo en tiempo real.

<p align="center">
  <img src="assets/Chapter-4/flowsModeling5.jpg" width="650"/>
</p>

La CryoGuard Platform detecta que hay conexión disponible y lo comunica a IoT Monitoring Management. Este restablece la conexión con Operations Management, que procede a sincronizar todos los datos almacenados con la nube. Al terminar, la plataforma actualiza el dashboard y entrega el historial de eventos completo al Operador Logístico.

### 4.1.1.3 Bounded Context Canvases.

En esta sección se presentan los Bounded Context Canvases definidos para el sistema, priorizando aquellos de mayor relevancia estratégica dentro del dominio de CryoGuard.

Su elaboración se realizó de forma iterativa, definiendo las responsabilidades, reglas de negocio y dependencias de cada módulo para asegurar una arquitectura desacoplada y eficiente.

#### **Bounded Context: Evaluation Management (Core)**
<p align="center">
  <img src="assets/Chapter-4/contextCanvases1.jpg" width="650"/>
</p>

#### **Bounded Context: IoT Monitoring Management**
<p align="center">
  <img src="assets/Chapter-4/contextCanvases2.jpg" width="650"/>
</p>

#### **Bounded Context: Operations Management (Flags)**

<p align="center">
  <img src="assets/Chapter-4/contextCanvases3.jpg" width="650"/>
</p>

#### **Bounded Context: Logistics Management**

<p align="center">
  <img src="assets/Chapter-4/contextCanvases4.jpg" width="650"/>
</p>

#### **Bounded Context: Actuation Management**

<p align="center">
  <img src="assets/Chapter-4/contextCanvases5.jpg" width="650"/>
</p>

#### **Bounded Context: Notification Management**

<p align="center">
  <img src="assets/Chapter-4/contextCanvases6.jpg" width="650"/>
</p>

#### **Bounded Context: IAM**

<p align="center">
  <img src="assets/Chapter-4/contextCanvases6.jpg" width="650"/>
</p>

### 4.1.2 Context Mapping.

En esta sección se presenta el Context Mapping del sistema, donde se analizan y definen las relaciones entre los bounded contexts identificados.

El diseño se realizó evaluando distintas alternativas de organización de capacidades, considerando su impacto en la cohesión, el acoplamiento y la complejidad del sistema. Asimismo, se aplicaron patrones de relación de Domain-Driven Design para establecer interacciones claras y consistentes entre contextos.

Finalmente, se seleccionó la aproximación más adecuada en función de la mantenibilidad, escalabilidad y claridad en la separación de responsabilidades.

<p align="center">
  <img src="assets/Chapter-4/contextMapping.jpg" width="650"/>
</p>

### 4.1.3.1 Software Architecture System Landscape Diagram

