# Checklist de secuencias del marco operativo
  
Esta es la lista de secuencias de intercambio que conforman el marco operativo de datos espaciales de la UA. Este apartado se organiza en secciones. Cada sección contiene información general acerca de una secuencia de intercambio de datos, y muestra en una tabla distintas variantes de la misma. Entre dichas variantes puede haber una que sea operativa, es decir, la que explica cómo se realiza el intercambio de datos actualmente. Los identificadores y descripciones de las secuencias son hiperenlaces a los correspondientes diagramas de secuencia. En estos diagramas se especifican en detalle los mensajes entre los distintos actores que participan en el intercambio.  

---
#### Recepción de ficheros CAD para actualización de geometría vectorial 2D
La actualización de la geometría en la base de datos geográfica de la UA se realiza, fundamentalmente, a partir de los planos de distribución de plantas y urbanización en formato digital, remitidos por el Servicio de Infraestructuras. En este sentido, la recepción de ficheros CAD relativos a obra nueva y reformas es el primer paso para ofrecer cartografía continua y coherente, tanto *indoor* como *outdoor*, del campus de San Vicente y las diversas sedes.

| Id | Descripción | Propuesta | En desarrollo | En pruebas | Operativo | En desuso |
| -- | -- | :--: | :--: | :--: | :--: | :--: |
| [ds01](ds01.md) | [Recepción de ficheros CAD por correo electrónico](ds01.md) | - | - | - | ✔ | - |
| [ds01-2](ds01-2.md) | [Recepción de ficheros CAD mediante tickets en un gestor de tareas](ds01-2.md) | ✔ | - | - | - | - |

---
#### Reparto de estancias
La adscripción de estancias a departamentos es un aspecto clave de la base de datos geográfica de la UA. La adscripción de estancias es competencia del Vicerrectorado de Campus y Sostenibilidad. Mantener actualizados los datos de adscripción permite, entre otras funcionalidades:  

-  Calcular estadísticas de superficie agregada.
-  Comparar valores de superficie entre la base de datos geográfica y el modelo de espacios.
-  Generar mapas de distribución de estancias por departamento.

| Id | Descripción | Propuesta | En desarrollo | En pruebas | Operativo | En desuso |
| -- | -- | :--: | :--: | :--: | :--: | :--: |
| [ds02](ds02.md) | [Adscripción de estancias a departamentos mediante sentencia SQL manual](ds02.md) | - | - | - | ✔ | - |
| [ds02-2](ds02-2.md) | [Aplicación HTML5 de adscripción de estancias a departamentos](ds02-2.md) | - | ✔ | - | - | - |

---
#### Asignación de usos de las estancias
La actividad habitual que se desempeña en una estancia es una cualidad fundamental de la base de datos geográfica de la UA. En cada departamento o unidad hay un miembro del PAS, previamente designado por el Vicerrectorado de Campus, que se encarga de indicar la actividad habitual de cada una de las estancias adscritas a ese departamento o unidad. Mantener actualizado el dato de actividad habitual permite articular un sistema de información de los usos del suelo construido de la UA, y tiene utilidades tales como:  

-  Reclasificar y agregar superficies según:
  -  El catálogo de usos del Servicio de Prevención.
  -  Criterios docentes.
  -  El sistema de auditoría de la CRUE.
-  Asignar automáticamente coeficientes de riesgo en el puesto de trabajo.
-  Comparar con los umbrales de superficie resultantes de aplicar el modelo de espacios.
-  Generar mapas de distribución de usos del suelo construido.
-  Confeccionar pliegos de condiciones para contratos de mantenimiento.

| Id | Descripción | Propuesta | En desarrollo | En pruebas | Operativo | En desuso |
| -- | -- | :--: | :--: | :--: | :--: | :--: |
| [ds03](ds03.md) | [Aplicación HTML5 de asignación de usos de las estancias](ds03.md) | - | - | - | ✔ | - |