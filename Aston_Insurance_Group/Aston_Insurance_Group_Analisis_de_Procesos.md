# Aston Insurance Group: Análisis de Operaciones y Procesos

**Preparado para:** Adriana Rubio, Aston Insurance Group
**Fecha:** 29 de enero de 2026
**Analista:** Analista de Crecimiento Operacional

---

## Sección 1: Resumen de Entendimiento del Negocio

Aston Insurance Group es una correduría de seguros con más de 20 años de experiencia sirviendo a la comunidad hispana en Florida y Texas a través de dos marcas distintas. La marca principal (Aston Insurance Group) ofrece una gama completa de productos que incluye seguros de vida, salud, accidentes, dental, visión, funerarios e internacionales, mientras que la marca secundaria (Seguro Con Obamacare) se enfoca específicamente en la inscripción de seguros de salud ACA/Marketplace. El negocio opera con una base de aproximadamente 3,000 clientes, la mayoría de los cuales tienen pólizas de seguro de salud.

El modelo operacional actual depende fuertemente del teléfono y es muy manual. La adquisición de clientes fluye principalmente a través de llamadas telefónicas entrantes y chat de WhatsApp, sin opciones de programación en línea ni autoservicio disponibles. La empresa utiliza ZOHO CRM pero reporta baja competencia y subutilización de sus capacidades. Una porción significativa del tiempo de los agentes se consume en tareas reactivas y repetitivas: verificar manualmente el portal del Marketplace de Healthcare.gov para solicitudes de documentos, monitorear el estado de pagos de clientes que optaron por no usar pago automático, y enviar mensajes de texto de seguimiento individuales uno por uno. No existe un enfoque sistemático para marketing de ciclo de vida (cumpleaños, disparadores por edad para elegibilidad de Medicare a los 65), venta cruzada a clientes existentes, ni comunicaciones automatizadas de renovación.

El negocio enfrenta presión creciente por los costos de adquisición de clientes en aumento, cambios en las pólizas ACA que han contribuido a la pérdida de clientes, y la ineficiencia fundamental de los procesos manuales que impiden que los agentes se enfoquen en actividades generadoras de ingresos. El liderazgo ha expresado claro interés en automatización para comunicaciones personalizadas masivas por SMS/correo electrónico, flujos de trabajo activados por edad, mecanismos mejorados de retención, y venta cruzada sistemática para maximizar el valor de por vida de su base de datos existente de 3,000 clientes.

---

## Sección 2: Brechas de Información

### Operaciones y Flujos de Trabajo
- No hay SOPs documentados para los flujos de trabajo diarios de los agentes (verificación de pólizas, secuencias de seguimiento de pagos)
- Frecuencia y volumen desconocido de solicitudes de documentos del Marketplace por día/semana
- No está claro cómo los agentes actualmente rastrean qué clientes necesitan seguimiento (¿hoja de cálculo? ¿ZOHO? ¿memoria?)
- Sin visibilidad del proceso de verificación de pólizas (¿qué portal? ¿cuántos clientes verificados diariamente?)
- Asignación de tiempo desconocida por agente entre diferentes categorías de tareas

### Ventas y Gestión de Prospectos
- No hay datos sobre fuentes actuales de prospectos y su volumen/calidad relativa
- Tasa de conversión de prospecto a cliente y duración del ciclo de ventas desconocidos
- No está claro cómo se distribuyen actualmente los prospectos entre agentes
- Sin información sobre el proceso de cotización (¿comparaciones manuales? ¿portales de aseguradoras?)
- Promedio desconocido de pólizas por cliente (penetración de venta cruzada)

### Datos de Clientes y Segmentación
- Sin desglose de los 3,000 clientes por tipo de producto, antigüedad o nivel de valor
- Porcentaje desconocido de clientes en pago automático vs. pago manual
- Sin visibilidad de las preferencias de comunicación de los clientes (SMS vs. correo vs. teléfono)
- No está claro cómo se rastrean actualmente los cumpleaños y fechas de nacimiento en ZOHO
- Sin datos sobre tasas de renovación de clientes por línea de producto

### Tecnología y Sistemas
- Sin información detallada de configuración de ZOHO (qué módulos están activos, qué datos se capturan)
- Capacidades de integración desconocidas entre ZOHO y otros sistemas
- Sin información sobre el sistema telefónico actual (¿VoIP? ¿seguimiento de llamadas?)
- No está claro qué datos existen en ZOHO vs. dispersos en hojas de cálculo/otras ubicaciones
- Sin visibilidad del uso de WhatsApp (¿cuentas personales? ¿WhatsApp Business? ¿API?)

### Estructura del Equipo
- Número desconocido de agentes y sus especializaciones
- Sin claridad sobre quién maneja Medicare vs. ACA vs. otros productos
- Estructura de reportes y procesos de supervisión gerencial poco claros
- Sin información sobre métricas de desempeño actuales o KPIs rastreados

### Cumplimiento y Restricciones
- Requisitos regulatorios desconocidos para comunicaciones automatizadas en seguros
- Sin información sobre requisitos de cumplimiento específicos de aseguradoras
- Consideraciones de privacidad de datos poco claras para la comunidad de inmigrantes hispanos

---

## Sección 3: Cuestionario para el Cliente

### A. Estructura del Equipo y Organización

1. ¿Cuántos agentes licenciados trabajan actualmente en Aston Insurance Group y cuáles son sus especializaciones principales de productos (ACA, Medicare, Vida, etc.)?

2. ¿Cómo es el horario diario típico de un agente? Por favor estime las horas dedicadas a: verificación de estado de pólizas, seguimientos de pagos, llamadas entrantes, llamadas de ventas salientes, tareas administrativas.

3. ¿Quién es responsable de gestionar ZOHO CRM y algún personal ha recibido capacitación formal en la plataforma?

4. ¿Tienen personal dedicado para marketing, servicio al cliente o soporte administrativo separado de los agentes licenciados?

### B. Procesos Actuales - Monitoreo de Pólizas

5. ¿Cuántas pólizas de clientes verifican los agentes diaria/semanalmente para solicitudes de documentos del Marketplace? ¿Cuál es el volumen típico de solicitudes de documentos encontradas por día?

6. Describa los pasos exactos que un agente toma cuando descubre una solicitud de documentos del Marketplace. ¿Qué sucede desde el descubrimiento hasta la resolución?

7. ¿Cómo rastrean actualmente los agentes qué pólizas han sido verificadas y cuáles aún necesitan atención? ¿Hay un sistema o se basa en la memoria?

8. ¿Qué porcentaje de sus 3,000 clientes son pólizas ACA/Marketplace vs. otros tipos de productos?

### C. Procesos Actuales - Seguimiento de Pagos

9. ¿Qué porcentaje de clientes están en pago automático vs. pago manual?

10. ¿Cómo identifican actualmente los agentes qué clientes tienen pagos atrasados o próximos? ¿Qué sistema o reporte utilizan?

11. ¿Cuántos mensajes de texto individuales se envían por día/semana para seguimientos de pagos?

12. ¿Cuál es su método actual de mensajes de texto (teléfono personal, línea de negocios, plataforma SMS)?

13. ¿Cuál es la secuencia típica de intentos de seguimiento antes de que una póliza caduque? ¿Cuántos puntos de contacto en qué período de tiempo?

### D. Ventas y Gestión de Prospectos

14. ¿Cuáles son sus fuentes actuales de prospectos y el volumen mensual aproximado de cada una (llamadas del sitio web, referencias, visitas, campañas de marketing)?

15. Cuando un nuevo prospecto llama, ¿qué información se captura y dónde se registra?

16. ¿Cuál es su tasa estimada de conversión de prospecto a cliente? ¿Cuánto tiempo toma el ciclo de ventas típico?

17. ¿Cómo comparan actualmente las opciones de pólizas para los clientes? ¿Usan portales de aseguradoras, software de cotización o comparaciones manuales?

18. ¿Qué venta cruzada ocurre actualmente? Cuando se incorpora un cliente de seguro de salud, ¿hay un proceso sistemático para ofrecer vida, dental u otros productos?

### E. Base de Datos de Clientes y ZOHO CRM

19. ¿Qué campos de datos de clientes están actualmente poblados en ZOHO (nombre, fecha de nacimiento, teléfono, correo electrónico, detalles de póliza, estado de pago, etc.)?

20. ¿Los cumpleaños y fechas de nacimiento de los clientes están capturados de manera confiable en ZOHO para los 3,000 clientes?

21. ¿Qué tan confiados están en la precisión de correos electrónicos y números de teléfono en su base de datos (estime el porcentaje)?

22. ¿Qué módulos/funciones de ZOHO están utilizando actualmente (Contactos, Negocios, Campañas, Flujos de Trabajo, etc.)?

23. ¿Hay datos importantes de clientes almacenados fuera de ZOHO (hojas de cálculo, archivos en papel, carpetas de correo electrónico)?

### F. Comunicación y Engagement

24. ¿Cuál es su actividad actual de marketing por correo electrónico? ¿Con qué frecuencia envían correos y qué herramientas utilizan?

25. ¿Tienen plantillas de correo electrónico o cada comunicación se escribe desde cero?

26. ¿Los clientes han proporcionado consentimiento para comunicaciones de marketing por SMS? ¿Cómo se capturó este consentimiento?

27. ¿En qué idiomas se comunican y esto varía por canal (teléfono vs. SMS vs. correo electrónico)?

### G. Tecnología e Integraciones

28. ¿Qué sistema telefónico utilizan? ¿Es VoIP y se integra con algún otro software?

29. ¿Su widget de WhatsApp está conectado a WhatsApp Business API o está redirigiendo a números de teléfono personales/de negocios?

30. ¿A qué portales de aseguradoras o sistemas externos acceden los agentes diariamente?

31. ¿Tienen alguna automatización o flujos de trabajo existentes configurados en ZOHO, aunque sean básicos?

### H. Métricas y Objetivos

32. ¿Cuál es su tasa actual de retención de clientes (porcentaje de clientes que renuevan anualmente)?

33. ¿Cuál es su objetivo de adquisición de nuevos clientes por mes?

34. Si pudieran liberar tiempo de los agentes de tareas manuales, ¿en qué querrían que se enfocaran?

35. ¿Cómo se ve el éxito en 12 meses? ¿Qué resultados específicos harían que esta inversión en automatización valga la pena?

---

## Sección 4: Mapa Preliminar de Procesos

| Proceso | Estado Actual | Tiempo/Frecuencia Est. | Dependencias | Potencial de Automatización |
|---------|---------------|------------------------|--------------|----------------------------|
| **Captura de Prospectos** | Llamadas telefónicas, chat WhatsApp; entrada manual en ZOHO | Volumen desconocido; ~5-10 min por prospecto | Sitio web, sistema telefónico, ZOHO | ALTO - Formularios web, captura automática, enrutamiento |
| **Calificación de Prospectos** | Conversación telefónica con agente | ~15-30 min por prospecto | Disponibilidad del agente | MEDIO - Chatbot/formularios de pre-calificación |
| **Cotización de Pólizas** | Comparaciones manuales en portales de aseguradoras | Desconocido; probablemente 20-45 min por cotización | Portales de aseguradoras, experiencia del agente | MEDIO - Integración de motor de cotización |
| **Incorporación de Clientes** | Entrada manual de datos, papeleo | Desconocido | Sistemas de aseguradoras, ZOHO | MEDIO - Formularios digitales, auto-población |
| **Monitoreo del Marketplace** | Verificaciones manuales diarias de Healthcare.gov | Alta frecuencia; tiempo desconocido por agente | Acceso al portal Healthcare.gov | ALTO - Integración API o RPA si está disponible |
| **Resolución de Solicitudes de Documentos** | Agente contacta cliente, recolecta docs, sube | Variable; ~30-60 min por caso | Capacidad de respuesta del cliente, acceso al portal | MEDIO - Alertas automatizadas, portal del cliente |
| **Monitoreo de Estado de Pagos** | Verificaciones manuales del estado de pago | Alta frecuencia; tiempo desconocido | Portales de aseguradoras/marketplace | ALTO - Monitoreo automatizado y alertas |
| **Seguimiento de Pagos (SMS)** | Textos individuales enviados uno por uno | Volumen desconocido; ~2-5 min cada uno | Teléfono personal, info de contacto del cliente | ALTO - SMS masivo con personalización |
| **Contacto por Cumpleaños** | No se hace actualmente | N/A | Datos de fecha de nacimiento en CRM | ALTO - Flujo de trabajo automatizado simple |
| **Disparador por Edad Medicare (65+)** | No se hace actualmente | N/A | Datos de fecha de nacimiento en CRM, especialista en Medicare | ALTO - Disparador de flujo de trabajo por edad |
| **Campañas de Venta Cruzada** | No se hace sistemáticamente | N/A | Datos de productos del cliente, segmentación | ALTO - Secuencias de nurturing automatizadas |
| **Recordatorios de Renovación** | Proceso actual desconocido | Anual por cliente | Fechas de vencimiento de pólizas | ALTO - Secuencia de recordatorios automatizada |
| **Engagement para Retención** | No se hace sistemáticamente | N/A | Historial del cliente, datos de engagement | MEDIO - Programa de lealtad, puntos de contacto regulares |

---

## Sección 5: Observaciones Iniciales

### Victorias Rápidas (Alto Impacto, Baja Complejidad)

1. **Correos/SMS Automatizados de Cumpleaños** - Si los datos de fecha de nacimiento existen en ZOHO, esto puede implementarse en días usando flujos de trabajo nativos de ZOHO o una integración simple. Constructor inmediato de buena voluntad con cero esfuerzo continuo.

2. **Implementación de Plataforma de SMS Masivo** - Reemplazar el envío de textos uno por uno con una plataforma como Twilio, SimpleTexting, o SMS integrado con ZOHO ahorrará horas semanales inmediatamente. Los recordatorios de pago pueden ser plantillas enviadas en lotes mientras aparecen personalizados.

3. **Flujo de Trabajo de Disparador por Edad Medicare** - Flujo de trabajo simple de ZOHO para marcar clientes que se acercan a los 65 y auto-asignar tareas al especialista en Medicare. Oportunidad de ingresos de bajo esfuerzo desde la base de clientes existente.

4. **Programación de Citas en Línea** - Agregar Calendly o similar a los sitios web captura prospectos que prefieren no llamar. La integración con ZOHO asegura que no haya entrada manual. Puede estar funcionando en una semana.

5. **Campaña de Correo por Goteo para Venta Cruzada** - Segmentar los 3,000 clientes existentes por productos actuales, crear secuencias simples de correo promoviendo cobertura complementaria. ZOHO Campaigns o integración con Mailchimp hace esto sencillo.

### Banderas Rojas y Áreas que Requieren Descubrimiento Más Profundo

1. **Preocupaciones sobre Calidad de Datos en ZOHO** - La admitida baja competencia con ZOHO sugiere que los datos de clientes pueden estar incompletos, inconsistentes o desactualizados. Cualquier automatización depende de datos confiables. Una auditoría de datos debe ser el primer paso antes de construir flujos de trabajo.

2. **Cuello de Botella en Monitoreo de Healthcare.gov** - Esto está consumiendo tiempo significativo de los agentes pero las opciones de automatización son limitadas por restricciones de acceso al portal. Necesitamos entender si el acceso API está disponible o si esto requiere RPA, lo cual aumenta la complejidad.

3. **Consentimiento SMS y Cumplimiento** - El marketing automatizado por SMS requiere consentimiento documentado (cumplimiento TCPA). Necesitamos verificar si el consentimiento existe y está debidamente registrado antes de implementar mensajería masiva.

4. **Arquitectura de WhatsApp** - Si WhatsApp está funcionando a través de cuentas personales en lugar de Business API, hay limitaciones de escalabilidad y cumplimiento que necesitarán abordarse.

5. **Riesgo de Punto Único de Falla** - La fuerte dependencia en procesos basados en teléfono con aparente falta de procedimientos documentados crea vulnerabilidad si personal clave no está disponible.

6. **Brecha en Marketing de Contenidos** - Blog no actualizado desde 2020 indica potenciales restricciones de recursos o descuido estratégico de la presencia digital. La automatización no resolverá problemas subyacentes de capacidad de contenido/marketing.

### Áreas de Enfoque Recomendadas para la Llamada de Descubrimiento

- Validar la calidad y completitud de datos en ZOHO (especialmente precisión de fecha de nacimiento, correo electrónico, teléfono)
- Entender el flujo de trabajo exacto de monitoreo de Healthcare.gov y explorar opciones de automatización
- Confirmar el estado de consentimiento SMS para la base de clientes existente
- Clarificar la capacidad de los agentes y hacia dónde se redirigiría el tiempo liberado
- Establecer métricas base (tasa de retención, tasa de conversión, tiempos de respuesta) para medir el impacto de la automatización
- Identificar restricciones de presupuesto y expectativas de cronograma

---

*Este análisis es preliminar y está basado únicamente en el documento de base de conocimiento proporcionado. Una llamada de descubrimiento será esencial para validar suposiciones, llenar brechas de información y priorizar iniciativas de automatización basadas en las restricciones y objetivos reales del negocio.*
