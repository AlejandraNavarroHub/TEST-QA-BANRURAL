### TESTEO

## ERRORES

### Correción linea 87

Descripción:
    El metodo *addEventListener()* estaba mal escrito, por esto al presionar el botón para verificar no realizaba ninguana acción.

Solución:
    Corregir la *e* en Event por *E*.

### Correción para generar el número aleatorio

Descripción:
    De la forma *Math.random() * 10* el número obtenido contendrá decimales y nunca llegará al número 100.

Solución:
    Agregar el maximo y mínimo de esta forma *Math.floor(Math.random() * (100 - 1) + 1);* y con el uso de Math.floor se eliminarán los decimales.

### Corrección de mensajes a mostrar

Descripción:
    Cuando el número ingresado es mayor, muestra que es menor y cuando es menor, muestra que es mayor; Así como al ser iguales muestra que es incorrecto.

Solución:
    Corregir los mensajes de forma correcta.

### Correción línea 49

Descripción:
    La constante lowOrHi toma el valor de la clase *lowOrHi* pero al llamarlo, no incluía el punto document.querySelector(*'lowOrHi'*);.

Solución:
    Agregar el punto al llamar el valor de la clase *document.querySelector('.lowOrHi');*

### Eliminar el uso de lowOrHi

Descripción:
    Esta clase y variable se utiliza solamente para mostrar el mensaje de si es menor o mayor, lo cual es innecesario ya que se puede agregar en LastResult.

Solución:
   Eliminar linea 38, 49, 66 y reemplazar en las verificaciones de mayor y menor *lowOrHi.textContent ==* por *lastResult.textContent +=*

### Eliminar el triple signo igual

Descripción:
    En javascript la comparación *===* es un ternario, si no se cambia aunque el número ingresado sea correcto lo tomará como incorrecto.

Solución:
    Se cambia el triple igual por un doble igual *==* para verificar que los valores sean iguales.
## Agregar console.log() temporales

Para conocer el numero generado, se imprime el número con un console.log(), de esta forma se comprobarán los colores y mensajes a mostrar.
