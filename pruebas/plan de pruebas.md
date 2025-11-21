# Tabla de Casos de Prueba

| ID | Caso de Prueba                         | Objetivo                                                | Datos / Precondiciones                                  | Pasos | Resultado Esperado                                    | Tipo |
|----|-----------------------------------------|---------------------------------------------------------|----------------------------------------------------------|-------|--------------------------------------------------------|------|
| CP01 | Registro exitoso de usuario | Verificar que el sistema permita registrar usuarios nuevos correctamente. | - Usuario no debe existir. <br> - Nombre: Juan Pérez <br> - Email: juan@example.com <br> - Contraseña: Abc123** | 1. Ingresar a “Registrar usuario”. <br> 2. Completar campos. <br> 3. Pulsar “Registrar”. | El sistema registra al usuario y muestra “Registro exitoso”. | Funcional, Caja negra |
| CP04 | Búsqueda de libro existente | Validar que la búsqueda funcione correctamente. | Datos: “El principito”. | 1. Ingresar término en barra de búsqueda. <br> 2. Presionar Enter. | El libro aparece en resultados en menos de 2 segundos. | Funcional |
| CP08 | Intentar préstamo sin stock | Validar manejo de errores. | Libro con stock = 0. | 1. Intentar prestar libro sin stock. | Mensaje: “Libro no disponible”. | Funcional |
| CP10 | Crear reserva de libro | Comprobar reserva exitosa. | Libro disponible para reserva. | 1. Seleccionar libro. <br> 2. Pulsar “Reservar”. | Reserva registrada y mensaje confirmatorio. | Funcional |
