# Restaurante Maderos · Diagramas BPMN

**As-Is-corregido** contiene P01–P10, un proceso por archivo, con P01 como entrada. Se conserva el alcance del servicio actual. Para revisar el flujo integrado, abrir los diez archivos en el mismo proyecto. Se excluye la plantilla vacía.

**To-Be-piloto** contiene PIL01 como diagrama de alcance, PIL02 para preparación y entrega, PIL03 para agotados y cambios, PIL04 para contingencia y PIL05 como interfaz opcional de caja. El piloto interviene las actividades 9–23 del perfil, con registro acotado de adicionales y correcciones. No incluye la automatización del cobro ni la facturación.

Los modelos son descriptivos. El diseño conserva las marcas T3, T4 y T5 con su significado en PIL-SERV-01. Las asignaciones operativas ajustadas, el manejo de pedidos sin productos y la definición del lote deben contrastarse con la encargada antes de certificar el As-Is.

La versión corregida y la propuesta están en carpetas independientes. Para revisar los cambios en Camunda sin mezclar versiones, importar cada carpeta en un proyecto separado.

**Entrada integrada del piloto: PIL06.** PIL01 abre el detalle de la comanda. Los subprocesos de evento de PIL06 permiten atender adicionales e inconformidades sin interrumpir el servicio y tratar por separado la cancelación total. PIL05 concilia el consumo con el procedimiento vigente de caja con o sin consulta digital. La matriz `To-Be-piloto/Trazabilidad.csv` enlaza el perfil con los elementos del modelo.

El umbral de dos minutos sin acuse se propuso para la validación previa al piloto. El As-Is mantiene pendientes de confirmar con la encargada el reparto real de tareas de caja, la agrupación por lote y las responsabilidades corregidas. No se atribuye el registro de consumo a Aldelo sin evidencia documental.
