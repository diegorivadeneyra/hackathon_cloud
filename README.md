# hackathon_cloud

# Integrantes
- Brayan Gomero
- Diego Rivadeneyra
- Domenic Rincon
- Eliseo Velasquez
  
# Arquitectura de solucion

# Cumlpimiento de requerimientos

## 1. Registro y Autenticación de Usuarios

•  El sistema debe permitir registro e inicio de sesión mediante credenciales institucionales
• ✔️ Se debe distinguir entre roles: estudiante, personal administrativo y autoridad

## 2. Reporte de Incidentes

• ✔️ Los usuarios deben poder crear reportes indicando tipo, ubicación, descripción y nivel de urgencia
• ✔️ Cada incidente se almacena en una base de datos serverless (DynamoDB)
• ✔️ Se genera automáticamente un identificador único por reporte

## 3. Actualización y Seguimiento en Tiempo Real

• ✔️ El sistema actualiza el estado de incidentes en tiempo real usando WebSockets
• Notificaciones instantáneas cuando un incidente cambia de estado
• ✔️ Estados: pendiente, en atención, resuelto

## 4. Panel Administrativo

• ✔️ Visualizar un panel con todos los incidentes activos
• ✔️ Permitir filtrar, priorizar y cerrar reportes
• ✔️ Actualizaciones en tiempo real sin recargar la página

## 5. Orquestación de Flujos con Apache Airflow

• Clasificación automática de incidentes por tipo o urgencia
• Envío de notificaciones a áreas responsables
• Generación periódica de reportes estadísticos

## 6. Gestión de Notificaciones

• Alertas en tiempo real mediante WebSocket y notificaciones asíncronas (correo o SMS) según gravedad

## 7. Historial y Trazabilidad

• Historial completo de acciones (creación, actualizaciones, responsables, fecha y hora)

## 8. Escalabilidad y Resiliencia

• ✔️ Componentes serverless y escalables automáticamente

## 9. Análisis Predictivo y Visualización Inteligente (Opcional)

• Integrar modelo de machine learning entrenado en AWS SageMaker
• Identificar patrones, zonas de riesgo y tendencias de recurrencia
• Predicciones sobre tipos de incidentes más probables en áreas y horarios específicos

# Deploy
