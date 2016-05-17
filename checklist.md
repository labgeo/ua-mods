# Checklist de secuencias
  
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
| [ds02-2](ds02-2.md) | [Aplicación HTML5 de adscripción de estancias a departamentos](ds02-2.md) | ✔ | - | - | - | - |