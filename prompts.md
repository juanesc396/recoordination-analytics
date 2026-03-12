# VHasist Analytic Prompts

### Prompts en grok

1. Buenas! Me gustaria que tomes el rol de un Data Miner de un call center de asistencia vehicular. Tu tarea es generar un .csv sintetico con asistencias (1000 rows).
Cada fila va a representar un caso que se recoordinó o no, para ello vamos a establecer 2 columnas, “anulado” “cancelado activado” y “coordinado”. Los casos vueltos a coordinar deberian tener valor 1 en las columnas anulado o cancelado activado y 1 en coordinado. y El resto 0 en todas o 1 en solo una columna.
Otra de las columnas deberia tener un pequeño comentario en el que se indique la razon por la que se recoordina la asistencia. Los motivos pueden ser:
- “No pudimos comunicarnos con el asegurado”
- “El numero de telefono del socio era erroneo”.
- “Por capacidades operativas no pudimos responder al auxilio cuando llegó al lugar”.
- “El auxilio devolvió el servicio”
- “El vehiculo estaba sobre autopista consecionada y el auxilio no tiene permitido operar ahí”
- “Ubicacion de origen erronea”
- “Demora elevada del prestador”
    
    Te doy libertad para crear otros motivos. Lo que si necesito que simulen ser comentarios humanos sobre lo que sucedio, que varie el lenguaje, que relaten cosas que suceden, con lenguaje tecnico de una persona que trabaja en este lugar y atiende llamadas.
    Cada row debe tener una fecha en formato dd/mm/yy hh/mm:ss
    
2. Ajusta comentarios para mayor realismo. y devuelve el csv directamente.

---

### Prompts en vscode

1. Me gustaria que en este notebook creemos 3 graficos para mostrar como se dividen los costos operativos de casos recoordinados.
Los graficos tienen que tener una paleta de colores con:
[#ffdbea, #d8f5f6, #fff6d9, #d8f7df] y como principal #ff012b
Vamos a usar la libreria plotly para crearlos.
- Va a ser un grafico con 3 subplots, 2 en el primer row y 1 en el segundo
- El primero va a ser un pie que muestre como se dividen los casos por type, por cantidad
- El segundo un barras que haga un top costo por barra
- El tercero un histograma que muestre costo por hora del dia
1. Me gustaria que el grafico de barras haga un top de la suma por cada tipo, para obtener insights de la razon que causa mas costos
2. Podriamos agregar markdown para explicar de manera minimalista las etapas del codigo? en transform_data y analytics?