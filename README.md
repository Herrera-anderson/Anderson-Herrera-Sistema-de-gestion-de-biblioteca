# Anderson-Herrera-Sistema-de-gestion-de-bibloteca
 
## 1. Descripción del Caso

Una plataforma cuyo propósito es administrar correctamente los procesos de registro de usuarios, préstamo y devoluciones de libros para que todo aquel
que la necesite pueda verse beneficiado y sea capaz de solicitar los libros y materiales que necesite.

---

## 2. Objetivos del Sistema
- Agilizar los procesos de préstamo, devolución y reserva.
- Mantener control del catálogo y stock de libros disponibles.
- Registrar y autenticar usuarios de forma segura.
- Generar reportes históricos y estadísticos.
- Proporcionar una interfaz accesible y comoda de usar.

---

## 3. Requerimientos del Sistema

### Requerimientos Funcionales
- RF01:Gestion de usuario) El sistema debe ser capaz de registrar nuevos usuarios con diferentes tipos de datos, autenticación, darles almacenamiento y recordatorio de base de usuario. 
- RF02:Gestion del catalogo) El sistema debe ser instantáneo a la hora de hacer las búsquedas, registrar nuevos libros, a la hora de editar sus datos, marcar libros para registrarlos como no disponibles en caso de prestamos o perdidas y clasificar los libros por diferentes categorías.
- RF03: Prestamos y devoluciones) Registrar las perdidas, los préstamos y devoluciones con fechas indicadas de cuando se hagan las cosas.
- RF04: Reservas) debe quedar registrado cuando un libro es reservado para algún usuario especifico y dárselo en el momento acordado, también hay que bloquear el préstamo del mismo mientras no este disponible y avisar cuando vuelva a estarlo.
- RF05: Historial ) registrar el historial de préstamo de cada usuario y de los diferentes libros de forma inmediata, donde se generan reportes y se hace el seguimiento mediante herramientas como Excel y registrado mediante archivos como pdf.
- RF06: Seguridad) el sistema debe generar registros de actividad para el usuario y dar restricciones dependiendo de los diferentes roles, bloqueo tras intentos fallidos y demás.
- RF07: Notificaciones) el sistema generara correos y avisos al usuario para saber como esta el asunto con libros.

### Requerimientos No Funcionales
- RNF01: El tiempo de respuesta de búsqueda debe ser menor a 2 segundos.
- RNF02: El sistema debe ser seguro y proteger credenciales.
- RNF03: Disponibilidad mínima del 99%.
- RNF04: Interfaz intuitiva y adaptable a dispositivos móviles.
- RNF05: Código mantenible y modular.

---

##  4. Tabla de Pruebas (Casos resumidos)

| ID | Caso de Prueba | Objetivo | Datos / Precondiciones | Pasos | Resultado Esperado |
|----|----------------|----------|-------------------------|--------|---------------------|
| CP01 | Registro exitoso de usuario | Verificar registro correcto de usuarios nuevos | Usuario no existente. Datos: Juan Pérez, juan@example.com | 1. Abrir “Registrar usuario”. <br> 2. Llenar campos. <br> 3. Registrar. | El sistema muestra “Registro exitoso”. |
| CP04 | Búsqueda de libro existente | Validar búsqueda funcional | Libro: “El principito” | 1. Escribir término. <br> 2. Enter. | El libro aparece en menos de 2 segundos. |
| CP08 | Préstamo sin stock | Validar manejo de errores | Stock = 0 | 1. Intentar préstamo. | Mensaje: “Libro no disponible”. |
| CP10 | Crear reserva | Verificar registro de reserva | Libro disponible | 1. Seleccionar libro. <br> 2. Reservar. | Reserva creada y mensaje confirmatorio. |

---

## 5. Tipo de Mantenimiento Propuesto

### Mantenimiento Correctivo
Solución de errores detectados en módulos como préstamos, reservas o autenticación.

### Mantenimiento Preventivo
Revisión mensual de logs, optimización de base de datos, verificación de respaldos y rendimiento.

### Mantenimiento Perfectivo
Mejoras solicitadas por los usuarios: velocidad de búsqueda, interfaz, reportes adicionales.

### Mantenimiento Evolutivo
Integración con otros sistemas, nuevos módulos (multas, RFID, estadísticas avanzadas).

---

## 6. Reflexión sobre el Control de Versiones
El uso de control de versiones (GitHub) es esencial para:
- Registrar cambios del sistema de forma clara y organizada.
- Permitir trabajo colaborativo sin sobrescribir archivos.
- Mantener un historial completo de mejoras, errores y soluciones.
- Restaurar versiones anteriores en caso de fallos.
- Facilitar la documentación a través de commits descriptivos.

Github se convierte en una herramienta clave para la confiabilidad, la transparencia y la evolución del proyecto de manera profesional.
