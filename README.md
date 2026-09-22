💻 Rol 1: Dev / Código (Roger e Ian) Al asignar a dos personas a este rol, pueden hacer pair programming o revisión cruzada para asegurar que el código es robusto.

    Roger puede centrarse en la prueba de arranque y en comprobar la limpieza estructural del código en App.java (sin errores de sintaxis ni llaves desparejadas).

    Ian asume la integridad lógica, verificando las dependencias, comprobando que la aplicación no se rompe al inicio y asegurando que los métodos de autenticación devuelven correctamente los booleanos.

🛡️ Rol 2: SysAdmin / Seguridad (Dan) Este es un rol analítico y ofensivo que puede manejar un solo especialista enfocado. Dan actuará como el auditor del equipo.

    Dan será el encargado de intentar "romper" el sistema. Verificará que el config.properties oculta bien las credenciales, ejecutará los ataques con ' OR '1'='1 para confirmar que los PreparedStatements resisten, y bombardeará el sistema con valores nulos o vacíos para confirmar que las excepciones están controladas.

🗄️ Rol 3: DBA / QA & Soporte (Gabri y Raul) Este rol combina la gestión de infraestructura de base de datos con las pruebas finales y la entrega, por lo que dividir las tareas entre dos agilizará el cierre del proyecto.

    Gabri toma la parte de DBA: asegura que las conexiones JDBC usen try-with-resources para evitar fugas de memoria y verifica que la base de datos H2 en memoria arranca e inserta los datos sin arrojar SQLException.

    Raul asume la parte de QA & Soporte: ejecuta la suite Main.java, recopila las evidencias visuales/logs de los 4 OK para el profesor y redacta la guía de puesta en marcha en local de 2 líneas.
