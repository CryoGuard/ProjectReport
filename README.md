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
  <img src="assets/Chapter-4/contextCanvases7.jpg" width="650"/>
</p>

### 4.1.2 Context Mapping.

En esta sección se presenta el Context Mapping del sistema, donde se analizan y definen las relaciones entre los bounded contexts identificados.

El diseño se realizó evaluando distintas alternativas de organización de capacidades, considerando su impacto en la cohesión, el acoplamiento y la complejidad del sistema. Asimismo, se aplicaron patrones de relación de Domain-Driven Design para establecer interacciones claras y consistentes entre contextos.

Finalmente, se seleccionó la aproximación más adecuada en función de la mantenibilidad, escalabilidad y claridad en la separación de responsabilidades.

<p align="center">
  <img src="assets/Chapter-4/contextMapping.jpg" width="650"/>
</p>

### 4.1.3.1 Software Architecture System Landscape Diagram


## 4.2. Tactical-Level Domain-Driven Design

### 4.2.4. Bounded Context: Control y Actuación

#### 4.2.4.1. Domain Layer

El bounded context Control y Actuación se encarga de la ejecución de acciones automáticas y manuales sobre los actuadores del dispositivo.

| Tipo | Clase / Nombre | Descripción | Atributos / Valores clave |
| --- | --- | --- | --- |
| Aggregate | ActuationSession | Agregado raíz que modela una sesión de actuación | id, shipmentId, actuatorId, commands[], status, startedAt, completedAt |
| Root | Actuator | Root del agregado; gestiona actuadores y sus estados | — |
| Value Object | ActuatorCommand | Comando a ejecutar en un actuador | command (START_COOLING, STOP_COOLING, LOCK, UNLOCK, ALERT), parameters{}, priority |
| Value Object | DutyCycle | Ciclo de trabajo para actuadores variables | onTime, offTime, cycles, currentCycle |
| Value Object | LockState | Estado de bloqueo del sistema | isLocked, lockType, lockedBy, lockedAt |
| Value Object | CoolingMode | Modo de enfriamiento activo | mode (ACTIVE, PASSIVE, EMERGENCY), targetTemp, currentTemp |
| Value Object | ExecutionResult | Resultado de ejecución de comando | success, errorMessage, executedAt, output{} |
| Domain Service | SafetyInterlockManager | Gestiona bloqueos de seguridad | checkInterlocks(), applyLock(), releaseLock() |
| Domain Event | ActuatorCommandScheduled | Comando programado para ejecución | sessionId, command, scheduledAt |
| Domain Event | ActuatorCommandExecuted | Comando ejecutado | sessionId, command, result, executedAt |
| Domain Event | CoolingStarted | Enfriamiento iniciado | sessionId, mode, targetTemp |
| Domain Event | CoolingStopped | Enfriamiento detenido | sessionId, reason |
| Domain Event | SafetyLockApplied | Bloqueo de seguridad aplicado | sessionId, lockType, appliedBy, timestamp |
| Domain Event | ManualCommandRejected | Comando manual rechazado por safety interlock | sessionId, command, reason, timestamp |

#### 4.2.4.2. Interface Layer

| Tipo | Clase / Nombre | Descripción | Métodos / Endpoints principales |
| --- | --- | --- | --- |
| Controller | ActuatorController | Control de actuadores | POST /api/commands · GET /api/actuators/status |
| Controller | OverrideController | Override manual protegido | POST /api/commands/override · GET /api/commands/override/available |
| DTO (in) | CommandResource | Payload de comando | actuatorId, command, parameters{}, authorizedBy? |
| DTO (in) | OverrideRequestResource | Request de override con autorización | command, reason, authToken, actor |
| DTO (out) | ExecutionResponse | Respuesta de ejecución | sessionId, command, result, executedAt |
| DTO (out) | ActuatorStatusResource | Estado actual de todos los actuadores | actuators[], lockState, coolingMode |

#### 4.2.4.3. Application Layer

| Tipo | Clase / Nombre | Descripción | Métodos / Comandos manejados |
| --- | --- | --- | --- |
| Command Handler | ExecuteCommandHandler | Ejecuta comando en actuador | handle(ExecuteCommandCommand) |
| Command Handler | ScheduleCommandHandler | Programa comando para ejecución diferida | handle(ScheduleCommandCommand) |
| Command Handler | ApplyOverrideHandler | Aplica override manual autorizado | handle(ApplyOverrideCommand) |
| Command Handler | ReleaseInterlockHandler | Libera bloqueo de seguridad | handle(ReleaseInterlockCommand) |
| Event Handler | ActuationResultPublisher | Publica resultado a Operaciones | on(ActuatorCommandExecuted) |
| Event Handler | SafetyEventPublisher | Publica eventos de seguridad | on(SafetyLockApplied, ManualCommandRejected) |

#### 4.2.4.4. Infrastructure Layer

| Tipo | Clase / Nombre | Descripción | Notas Técnicas |
| --- | --- | --- | --- |
| Repository | ActuationRepository | Persistencia de sesiones y comandos | PostgreSQL |
| Mapper | ActuatorCommandMapper | Mapear comandos a instrucciones MCU | GPIO/PWM/UART |
| Messaging | CommandQueue | Cola de comandos con confirmación | Internal Queue |
| Hardware | ActuatorDriverAdapter | Adaptador para ESP32 | PWM, GPIO, MOSFET/relay para Peltier |
| Projection | ActuationHistoryReadModelRepository | Proyección para historial y auditoría | Vista materializada por shipmentId |

#### 4.2.4.5. Bounded Context Software Architecture Component Level Diagrams

![component-actuation](./assets/Chapter-4/control_actuacion_c4.png)

#### 4.2.4.6. Bounded Context Software Architecture Code Level Diagrams

##### 4.2.4.6.1. Bounded Context Domain Layer Class Diagrams

![class-actuation](./assets/Chapter-4/control_actuacion_uml.png)

##### 4.2.4.6.2. Bounded Context Database Design Diagram

![db-actuation](./assets/Chapter-4/control_actuacion_db.png)

### 4.2.5 Bounded Context: Operaciones / Flags

#### 4.2.5.1. Domain Layer

El bounded context Operaciones / Flags se encarga de la gestión de incidentes, decisiones humanas y overrides con trazabilidad completa.

| Tipo | Clase / Nombre | Descripción | Atributos / Valores clave |
| --- | --- | --- | --- |
| Aggregate | ColdChainIncident | Agregado raíz que modela un incidente de cadena de frío | id, shipmentId, flagId, state, decisions[], createdAt, resolvedAt |
| Root | IncidentCase | Root del agregado; gestiona el ciclo de vida del incidente | — |
| Value Object | DecisionType | Tipo de decisión sobre el producto | type (USE, TRANSFER, DISCARD, QUARANTINE) |
| Value Object | OverrideReason | Razón del override proporcionado | reason, category, evidenceRequired |
| Value Object | EvidenceReference | Referencia a evidencia del override | type (PHOTO, SIGNATURE, AUDIO), url, uploadedAt |
| Value Object | OperatorIdentity | Identidad del operador que toma decisiones | userId, name, role, authenticatedAt |
| Value Object | FlagState | Estado de la bandera asociada al incidente | status (OPEN, ACKNOWLEDGED, ESCALATED, CLOSED), severity |
| Domain Service | IncidentLifecycleManager | Gestiona el ciclo de vida de incidentes | openIncident(), acknowledge(), escalate(), close() |
| Domain Event | IncidentOpened | Incidente abierto a partir de flag | incidentId, flagId, shipmentId, openedAt |
| Domain Event | IncidentAcknowledged | Incidente reconocido por operador | incidentId, acknowledgedBy, acknowledgedAt |
| Domain Event | HandlingDecisionRecorded | Decisión de manejo registrada | incidentId, decision, operator, recordedAt |
| Domain Event | OverrideRegistered | Override registrado con motivo y actor | incidentId, overrideReason, actor, authorizedBy, timestamp |
| Domain Event | IncidentClosed | Incidente cerrado | incidentId, finalDecision, closedBy, closedAt |

#### 4.2.5.2. Interface Layer

| Tipo | Clase / Nombre | Descripción | Métodos / Endpoints principales |
| --- | --- | --- | --- |
| Controller | IncidentController | Gestión de incidentes | GET /api/incidents · GET /api/incidents/{id} |
| Controller | DecisionController | Registro de decisiones de manejo | POST /api/incidents/{id}/decisions |
| Controller | OverrideController | Registro de overrides | POST /api/incidents/{id}/override |
| DTO (in) | IncidentResource | Request de creación de incidente | flagId, shipmentId, initialSeverity |
| DTO (in) | DecisionResource | Request de decisión de manejo | decisionType, reasoning, evidence? |
| DTO (in) | OverrideResource | Request de override | reason, authToken, actor, evidence? |
| DTO (out) | IncidentResponse | Respuesta de incidente | id, shipmentId, flagId, state, decisions[], createdAt, resolvedAt |
| DTO (out) | DecisionResponse | Respuesta de decisión registrada | id, decisionType, operator, recordedAt |

#### 4.2.5.3. Application Layer

| Tipo | Clase / Nombre | Descripción | Métodos / Comandos manejados |
| --- | --- | --- | --- |
| Command Handler | OpenIncidentHandler | Abre incidente a partir de flag | handle(OpenIncidentCommand) |
| Command Handler | AcknowledgeIncidentHandler | Reconoce incidente | handle(AcknowledgeIncidentCommand) |
| Command Handler | RecordDecisionHandler | Registra decisión de manejo | handle(RecordDecisionCommand) |
| Command Handler | RegisterOverrideHandler | Registra override con trazabilidad | handle(RegisterOverrideCommand) |
| Command Handler | CloseIncidentHandler | Cierra incidente | handle(CloseIncidentCommand) |
| Event Handler | IncidentStatePublisher | Publica cambios de estado a Notificaciones | on(IncidentOpened, IncidentClosed) |
| Event Handler | DecisionAuditPublisher | Publica decisiones para auditoría | on(HandlingDecisionRecorded, OverrideRegistered) |

#### 4.2.5.4. Infrastructure Layer

| Tipo | Clase / Nombre | Descripción | Notas Técnicas |
| --- | --- | --- | --- |
| Repository | IncidentRepository | Persistencia de incidentes | SQLite/PostgreSQL |
| Mapper | IncidentJpaMapper | Mapear incidentes a entidades JPA | Colecciones embebidas para decisiones |
| Messaging | OutboxPublisher | Publicación transaccional de eventos | Tabla outbox + publicador async |
| Integration | NotificationACLClient | Envía eventos a Notificaciones | REST call |
| Projection | IncidentReadModelRepository | Proyección para dashboard y app | Vista materializada por shipmentId y estado |

#### 4.2.5.5. Bounded Context Software Architecture Component Level Diagrams

![component-operations](./assets/Chapter-4/operaciones_flag_c4.png)

#### 4.2.5.6. Bounded Context Software Architecture Code Level Diagrams

##### 4.2.5.6.1. Bounded Context Domain Layer Class Diagrams

![class-operations](./assets/Chapter-4/operaciones_flag_uml.png)

##### 4.2.5.6.2. Bounded Context Database Design Diagram

![db-operations](./assets/Chapter-4/operaciones_flag_db.png)

### 4.2.6 Bounded Context: Notificaciones

#### 4.2.6.1. Domain Layer

El bounded context Notificaciones se encarga de la entrega de alertas a través de múltiples canales.

| Tipo | Clase / Nombre | Descripción | Atributos / Valores clave |
| --- | --- | --- | --- |
| Aggregate | Alert | Agregado raíz que gestiona alertas y su ciclo de vida | id, type, severity, message, shipmentId, status, channelsSent[], attempts, createdAt, acknowledgedAt, acknowledgedBy |
| Value Object | Channel | Canal de notificación | type (DASHBOARD, EMAIL, LOCAL_DISPLAY) |
| Value Object | AlertStatus | Estado de la alerta | status (NEW, SENT, ACKNOWLEDGED) |
| Value Object | Severity | Severidad de la alerta | level (INFO, WARNING, CRITICAL) |
| Domain Service | NotificationDispatcher | Dispatcha alertas a los canales configurados | dispatch(), sendToChannel() |
| Domain Event | AlertCreated | Alerta creada a partir de evento del dominio | alertId, type, severity, shipmentId, createdAt |
| Domain Event | AlertSent | Alerta enviada a canal | alertId, channel, sentAt |
| Domain Event | AlertAcknowledged | Alerta reconocida por operador | alertId, acknowledgedBy, acknowledgedAt |

#### 4.2.6.2. Interface Layer

| Tipo | Clase / Nombre | Descripción | Métodos / Endpoints principales |
| --- | --- | --- | --- |
| Controller | AlertController | Gestión de alertas | GET /api/alerts · POST /api/alerts · GET /api/alerts/{id} |
| DTO (in) | CreateAlertRequest | Request de creación de alerta | type, severity, shipmentId, message |
| DTO (in) | AcknowledgeAlertRequest | Request de reconocimiento | acknowledgedBy |
| DTO (out) | AlertResponse | Respuesta de alerta | id, type, severity, message, shipmentId, status, channelsSent, attempts, createdAt, acknowledgedAt, acknowledgedBy |
| DTO (out) | AlertListResponse | Lista de alertas | alerts[], total, page |

#### 4.2.6.3. Application Layer

| Tipo | Clase / Nombre | Descripción | Métodos / Comandos manejados |
| --- | --- | --- | --- |
| Command Handler | CreateAlertHandler | Crea nueva alerta | handle(CreateAlertCommand) |
| Command Handler | SendAlertHandler | Envía alerta a canales | handle(SendAlertCommand) |
| Command Handler | AcknowledgeAlertHandler | Reconoce alerta | handle(AcknowledgeAlertCommand) |
| Command Handler | RetryAlertHandler | Reintenta envío de alerta fallida | handle(RetryAlertCommand) |
| Event Handler | AlertEventPublisher | Publica alertas criadas | on(AlertCreated) |
| Event Handler | AlertNotificationSubscriber | Suscribe a eventos de otros contextos | on(FlagRaised, OverrideRegistered) |

#### 4.2.6.4. Infrastructure Layer

| Tipo       | Clase / Nombre           | Descripción                      | Notas Técnicas                  |
| ---------- | ------------------------ | -------------------------------- | ------------------------------- |
| Repository | AlertRepository          | Persistencia de alertas          | PostgreSQL                      |
| Messaging  | WebSocketGateway         | Gateway WebSocket para dashboard | Spring WebSocket                |
| Email      | EmailNotificationAdapter | Adaptador para envío de emails   | JavaMailSender simple           |
| Local      | LocalDisplayAdapter      | Adaptador para pantalla local    | Envío de alertas a edge display |
| Projection | AlertReadModelRepository | Proyección para dashboard        | Query by shipmentId y status    |

#### 4.2.6.5. Bounded Context Software Architecture Component Level Diagrams

![component-notifications](./assets/Chapter-4/notificaciones_c4.png)

#### 4.2.6.6. Bounded Context Software Architecture Code Level Diagrams

##### 4.2.6.6.1. Bounded Context Domain Layer Class Diagrams

![class-notifications](./assets/Chapter-4/notificaciones_uml.png)

##### 4.2.6.6.2. Bounded Context Database Design Diagram

![db-notifications](./assets/Chapter-4/notificaciones_db.png)

### 4.2.7. Bounded Context: Seguridad / Roles

#### 4.2.7.1. Domain Layer

El bounded context Seguridad / Roles se encarga de la identidad, autenticación, autorización y auditoría de acceso.

| Tipo | Clase / Nombre | Descripción | Atributos / Valores clave |
| --- | --- | --- | --- |
| Aggregate | AccessControlContext | Agregado raíz que modela el contexto de control de acceso | id, tenantId, policies[], roles[], deviceTrusts[] |
| Root | User | Root del agregado; gestiona usuarios y sus permisos | — |
| Value Object | Role | Rol con permisos asociados | roleId, name, permissions[], scope |
| Value Object | Permission | Permiso específico | permissionId, resource, action, constraints{} |
| Value Object | AuthToken | Token de autenticación | tokenId, userId, issuedAt, expiresAt, scope |
| Value Object | ApprovalScope | Alcance de aprobación temporal | scope, maxDuration, allowedActions[] |
| Domain Service | AuthorizationResolver | Resuelve permisos para acciones específicas | resolvePermission(), checkAccess() |
| Domain Service | TokenManager | Gestiona emisión y validación de tokens | issueToken(), validateToken(), revokeToken() |
| Domain Event | UserAuthenticated | Usuario autenticado exitosamente | userId, method, authenticatedAt, deviceId? |
| Domain Event | RoleGranted | Rol asignado a usuario | userId, role, grantedBy, grantedAt |
| Domain Event | OverrideAuthorized | Override autorizado | userId, scope, authorizedBy, expiresAt |
| Domain Event | AccessDenied | Acceso denegado | userId, resource, action, reason, timestamp |
| Domain Event | DeviceRegistered | Dispositivo registrado en el sistema | deviceId, deviceType, registeredAt, trustLevel |

#### 4.2.7.2. Interface Layer

| Tipo | Clase / Nombre | Descripción | Métodos / Endpoints principales |
| --- | --- | --- | --- |
| Controller | AuthController | Autenticación de usuarios | POST /api/auth/login · POST /api/auth/logout · POST /api/auth/refresh |
| Controller | AuthorizationController | Autorización y permisos | POST /api/auth/authorize · GET /api/auth/permissions |
| Controller | DeviceController | Registro y gestión de dispositivos | POST /api/auth/devices · GET /api/auth/devices/{id} |
| DTO (in) | LoginResource | Request de login | username, password, deviceInfo? |
| DTO (in) | AuthorizeResource | Request de autorización | resource, action, context{} |
| DTO (in) | DeviceRegistrationResource | Request de registro de dispositivo | deviceType, fingerprint, metadata{} |
| DTO (out) | TokenResponse | Respuesta de token | accessToken, refreshToken, expiresAt |
| DTO (out) | AuthorizationResponse | Respuesta de autorización | allowed, reason, constraints{} |
| DTO (out) | DeviceResponse | Respuesta de dispositivo | deviceId, status, trustLevel, registeredAt |

#### 4.2.7.3. Application Layer

| Tipo | Clase / Nombre | Descripción | Métodos / Comandos manejados |
| --- | --- | --- | --- |
| Command Handler | AuthenticateUserHandler | Autentica usuario | handle(AuthenticateUserCommand) |
| Command Handler | GrantRoleHandler | Asigna rol a usuario | handle(GrantRoleCommand) |
| Command Handler | AuthorizeOverrideHandler | Autoriza override temporal | handle(AuthorizeOverrideCommand) |
| Command Handler | RegisterDeviceHandler | Registra dispositivo | handle(RegisterDeviceCommand) |
| Command Handler | RevokeTokenHandler | Revoca token | handle(RevokeTokenCommand) |
| Event Handler | AccessAuditPublisher | Publica eventos de auditoría | on(UserAuthenticated, AccessDenied, OverrideAuthorized) |
| Event Handler | DeviceStatePublisher | Publica estado de dispositivo | on(DeviceRegistered) |

#### 4.2.7.4. Infrastructure Layer

| Tipo | Clase / Nombre | Descripción | Notas Técnicas |
| --- | --- | --- | --- |
| Repository | UserRepository | Persistencia de usuarios | SQLite/PostgreSQL con cifrado de password |
| Repository | PolicyRepository | Persistencia de políticas | SQLite/PostgreSQL |
| Mapper | UserJpaMapper | Mapear usuarios a entidades JPA | Conversión de roles y permisos |
| Security | JwtValidator | Validador de JWT | Verificación de firma y expiración |
| Security | SimpleAuthProvider | Proveedor de autenticación simple | Basic auth o JWT simple |
| Projection | AuditLogRepository | Proyección para logs de auditoría | Vista materializada por userId y timestamp |

#### 4.2.7.5. Bounded Context Software Architecture Component Level Diagrams

![component-security](./assets/Chapter-4/seguridad_roles_c4.png)

#### 4.2.7.6. Bounded Context Software Architecture Code Level Diagrams

##### 4.2.7.6.1. Bounded Context Domain Layer Class Diagrams

![class-security](./assets/Chapter-4/seguridad_roles_uml.png)

##### 4.2.7.6.2. Bounded Context Database Design Diagram

![db-security](./assets/Chapter-4/seguridad_roles_db.png)
