# Diagramas de secuencia

El marco operativo de datos espaciales de la UA se define como un conjunto de diagramas de secuencia. Se trata de un tipo concreto de diagramas de interacción que permiten comunicar e interpretar fácilmente cómo funciona un proceso.  

Estos diagramas se componen básicamente de:  
- Rectángulos que representan **actores**.
- Flechas de línea sólida que representan **mensajes emitidos** por un actor.
- Flechas de línea discontinua que representan **respuestas** a un mensaje previo.  

Los mensajes de un diagrama de secuencia se leen de arriba hacia abajo, dado que están ordenados siguiendo una línea temporal.  

Veamos un ejemplo de cómo representar en un diagrama de secuencia el siguiente proceso:  
> El usuario se identifica en UACloud con su cuenta de usuario @ua.es, abre la aplicación, accede a la lista de estancias, selecciona una estancia y actualiza la actividad habitual a la que está destinada. Cuandos los cambios se aplican, la aplicación muestra un mensaje informativo.  

El diagrama es el siguiente:  

{% mermaid %}
sequenceDiagram
Usuario->>UACloud:se identifica con su cuenta de usuario @ua.es;
Usuario->>App:accede a la lista de estancias;
Usuario->>App:selecciona una estancia;
Usuario->>App:edita actividad habitual;
Usuario->>App:acepta los cambios;
App-->>Usuario:muestra un mensaje informativo;
{% endmermaid %}

Y este es el código mediante el que definimos el diagrama:  

```
{% mermaid %}
sequenceDiagram
Resp. espacios->>UACloud:se identifica con su cuenta de usuario @ua.es;
Resp. espacios->>App:accede a la lista de estancias;
Resp. espacios->>App:selecciona una estancia;
Resp. espacios->>App:edita actividad habitual;
Resp. espacios->>App:acepta los cambios;
App-->>Resp.espacios:muestra un mensaje informativo;
{% endmermaid %}
```

### Observaciones sobre las denominaciones de los actores
-  Se utilizan diagramas de secuencia simplificados en los que un actor puede hacer referencia tanto a usuarios como a componentes de software. Los usuarios pueden ser todos los pertenecientes a un colectivo u organismo (e.g. Vic. Campus) como usuarios individuales (e.g. Técnico SIGUA). A su vez, un componente de software puede ser tanto una aplicación concreta como un servicio o plataforma de servicios (e.g. UACloud).
-  Cuando se menciona el actor `Resp. espacios` siempre se hace referencia al gestor PAS responsable de espacios de su departamento o unidad.
-  Cuando se menciona el actor `Base de datos` siempre nos referimos a la base de datos geográfica de la UA.