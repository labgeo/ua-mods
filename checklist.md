# Checklist de secuencias del marco operativo
  
Esta es la lista de secuencias de intercambio que conforman el marco operativo de datos espaciales de la UA. Este apartado se organiza en secciones. Cada sección contiene información general acerca de una secuencia de intercambio de datos, y muestra en una tabla distintas variantes de la misma. Entre dichas variantes puede haber una que sea operativa, es decir, la que explica cómo se realiza el intercambio de datos actualmente. Los identificadores y descripciones de las secuencias son hiperenlaces a los correspondientes diagramas de secuencia. En estos diagramas se especifican en detalle los mensajes entre los distintos actores que participan en el intercambio.  

<!--sec data-title="Recepción de ficheros CAD para actualización de geometría vectorial 2D" data-id="01" ces-->

La actualización de la geometría en la base de datos geográfica de la UA se realiza, fundamentalmente, a partir de los planos de distribución de plantas y urbanización en formato digital, remitidos por el Servicio de Infraestructuras. En este sentido, la recepción de ficheros CAD relativos a obra nueva y reformas es el primer paso para ofrecer cartografía continua y coherente, tanto *indoor* como *outdoor*, del campus de San Vicente y las diversas sedes.

| Id | Descripción | Propuesta | En desarrollo | En pruebas | Operativo | En desuso |
| -- | -- | :--: | :--: | :--: | :--: | :--: |
| [ds01](ds01.md) | [Recepción de ficheros CAD por correo electrónico](ds01.md) | - | - | - | ✔ | - |
| [ds01-2](ds01-2.md) | [Recepción de ficheros CAD mediante tickets en un gestor de tareas](ds01-2.md) | ✔ | - | - | - | - |

<!--endsec-->

<!--sec data-title="Reparto de estancias" data-id="02" ces-->

La adscripción de estancias a departamentos es un aspecto clave de la base de datos geográfica de la UA. La adscripción de estancias es competencia del Vicerrectorado de Campus y Sostenibilidad. Mantener actualizados los datos de adscripción permite, entre otras funcionalidades:  

-  Calcular estadísticas de superficie agregada.
-  Comparar valores de superficie entre la base de datos geográfica y el modelo de espacios.
-  Generar mapas de distribución de estancias por departamento.

| Id | Descripción | Propuesta | En desarrollo | En pruebas | Operativo | En desuso |
| -- | -- | :--: | :--: | :--: | :--: | :--: |
| [ds02](ds02.md) | [Adscripción de estancias a departamentos mediante sentencia SQL manual](ds02.md) | - | - | - | ✔ | - |
| [ds02-2](ds02-2.md) | [Aplicación HTML5 de adscripción de estancias a departamentos](ds02-2.md) | - | ✔ | - | - | - |

<!--endsec-->

<!--sec data-title="Asignación de usos de las estancias" data-id="03"  ces-->

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

<!--endsec-->

<!--sec data-title="Ubicación de puestos de trabajo" data-id="04"  ces-->

Junto con la adscripción de departamentos y la asignación de actividad habitual de las estancias, la ubicación de puestos de trabajo es el tercer aspecto que caracteriza a la base de datos geográfica de la UA. El mismo gestor que asigna la actividad habitual de las estancias, se encarga a su vez de indicar en qué estancias desempeñan su puesto el PAS, el PDI y los cargos de su departamento o unidad. Además de hacer posible la localización geográfica desde el directorio de personal, el dato de ubicación permite que el Servicio de Prevención incorpore automáticamente al perfil de salud laboral del trabajador los factores de riesgo derivados del lugar en el que desempeña su puesto.

| Id | Descripción | Propuesta | En desarrollo | En pruebas | Operativo | En desuso |
| -- | -- | :--: | :--: | :--: | :--: | :--: |
| [ds04](ds04.md) | [Aplicación HTML5 de ubicación de puestos de trabajo](ds04.md) | - | - | - | ✔ | - |

<!--endsec-->

<!--sec data-title="Designación de PAS responsable de espacios" data-id="05" ces-->

El Vicerrectorado de Campus, de común acuerdo con los departamentos y unidades, es el órgano competente para designar al gestor PAS responsable de espacios de cada departamento o unidad. Los responsables de espacios tienen 2 funciones fundamentales de cara a la actualización de la base de datos geográfica de la UA:  

-  Asignar la actividad habitual a la que se destina cada estancia de su respectivo departamento o unidad.
-  Ubicar al PAS, al PDI y a los cargos de su respectivo departamento o unidad.

| Id | Descripción | Propuesta | En desarrollo | En pruebas | Operativo | En desuso |
| -- | -- | :--: | :--: | :--: | :--: | :--: |
| [ds05](ds05.md) | [Designación de PAS responsable de espacios mediante sentencia SQL manual](ds05.md) | - | - | - | ✔ | - |
| [ds05-2](ds05-2.md) | [App HTML5 para la designación de PAS responsable de espacios](ds05-2.md) | - | - | ✔ | - | - |

<!--endsec-->

<!--sec data-title="Auto-ubicación de puestos de trabajo" data-id="06"  ces-->

En algunos casos, el responsable de espacios no puede ubicar con exactitud los puestos de trabajo de su departamento o unidad. Esto puede ser debido a que el personal trabaja en dependencias dispersas o incluso en estancias que no están adscritas a su departamento. Para evitar omisiones o inconsistencias en los datos de ubicación, se requiere un mecanismo simple y seguro que permita al PAS o al PDI notificar a su responsable de espacios dónde desempeña su puesto. A esta utilidad la denominamos auto-ubicación porque permite al propio PAS o PDI iniciar el proceso de actualización de su lugar de trabajo en la base de datos geográfica de la UA.

| Id | Descripción | Propuesta | En desarrollo | En pruebas | Operativo | En desuso |
| -- | -- | :--: | :--: | :--: | :--: | :--: |
| [ds06](ds06.md) | [Aplicación HTML5 de auto-ubicación de puestos de trabajo](ds06.md) | - | - | - | ✔ | - |

<!--endsec-->

<!--sec data-title="Integración de datos organizativos y de personal" data-id="07" ces-->

Los datos de estructura organizativa (unidades, subunidades, centros y departamentos docentes) y de personal (PDI, PAS y cargos) se replican periódicamente en la base de datos geográfica de la UA a partir de las bases de datos corporativas de gestión de personal. Por tanto, una vez replicados, son tratados como datos de sólo lectura.

| Id | Descripción | Propuesta | En desarrollo | En pruebas | Operativo | En desuso |
| -- | -- | :--: | :--: | :--: | :--: | :--: |
| [ds07](ds07.md) | [Aplicación de escritorio para la copia incremental de datos organizativos y de personal](ds07.md) | - | - | - | ✔ | - |

<!--endsec-->

<!--sec data-title="Versionado de datos" data-id="08" ces-->
El control de versiones de datos es un mecanismo independiente del de copias de seguridad. Gracias al versionado de datos es posible realizar el seguimiento de los cambios realizados en la geometría, la actividad habitual y la adscripción de una estancia, así como en la ubicación de un puesto de trabajo. En este sentido, se puede responder a preguntas del tipo:  
-  ¿Qué modificaciones geométricas ha sufrido esta estancia?
-  ¿Cuál era previamente la actividad habitual de esta estancia?
-  ¿A qué departamento pertenecía anteriormente esta estancia?
-  ¿En qué estancia se ubicaba este puesto de trabajo antes?

<!--endsec-->