# generador-crucigrama
Este repositorio contiene una página web diseñada para crear y resolver crucigramas interactivos. 

El proyecto fue desarrollado utilizando HTML, CSS y JavaScript e incorpora un algoritmo para organizar e intersectar las palabras dentro del tablero.

El algoritmo funciona de la siguiente forma:

Primero, solicita los conceptos junto con las pistas y posteriormente se limpia el texto antes de mostrarlo en la página de manera que si el usuario escribe caracteres que HTML pueda interpretar como código se muestren solamente como texto.

Ya que se ingresaron los conceptos, se ordenan los conceptos de mayor a menor números de letras y así agregarlo al centro del crucigrama y comparar las letras de todos los conceptos para encontrar similitudes para ordenarlos de manera horizontal y vertical. 

Se generan 80 crucigramas como posibles candidatos ya que cada crucigrama generado se le asigna un puntaje que va a depender si cada crucigrama no obtuvo errores al generar el crucigrama con el mayor puntaje es la que se presenta para poder exportarlo.

Al exportarlo a HTML todas las respuestas se convierte a mayúscula y recorre palabra por palabra obteniendo el valor numérico que le corresponde cada carácter guardándolo en una constante mediante filas y columnas almacenando en el valor hasheado en las celdas como arreglo donde cada objeto representa una palabra que contiene su valor numérico ordenándolo  en valores de X, Y con la longitud que le corresponde para que cuando el usuario verifique sus respuestas se compare el valor numérico con el valor hasheado en las posiciones de las celdas la cuál está ubicado en X, Y si la respuesta es correcta le da un puntaje la cual irá sumándose hasta que todas las respuestas sean correctas.

Si la respuesta es incorrecta el recuadro se pondrá en rojo y le marcara con un mensaje si la respuesta es incorrecta, en el caso que le faltara o se pasara de palabra a tu respuesta le dará el mensaje de que no cumple con el número de letras esperados.

Al terminar de responder de manera correcta el crucigrama le dará un mensaje de felicitaciones.
