# Apuntes de markdown

## Titulos

Para crear titulos se usa el caracter `#` seguido de un espacio y el texto del titulo.

Mientras mas `#` se usen mas pequeño sera el titulo.

## Saltos de linea

Basta con dejar una linea en blanco entre dos lineas de texto.

## Citas

Para crear citas se usa el caracter `>` seguido de un espacio y el texto de la cita.

> Esto es una cita

## Listas

### Listas desordenadas

- Con un guíon `-` seguido de un espacio y el texto de la lista.
- Algunas aplicaciones aceptan el caracter `*` o `+` en lugar de `-`.
  
### Listas ordenadas

1. Con un numero seguido de un punto `.` seguido de un espacio y el texto de la lista.
2. El numero no tiene que ser secuencial.

    2.1 Se pueden crear sub listas con 4 espacios antes del texto.

    2.a Se pueden usar letras en lugar de numeros.

### Listas de tareas

- [x] Tarea completada
- [ ] Tarea pendiente
  
## Separadores

Si uso `___` markdown creará una linea horizontal.
___

## Negritas y cursivas

*Cursiva*: Se usa un asterisco `*` o un guion bajo `_` antes y despues del texto.

**Negrita**: Se usa dos asteriscos `**` o dos guiones bajos `__` antes y despues del texto.

***Cursiva y negrita***: Se usa tres asteriscos `***` o tres guiones bajos `___` antes y despues del texto.

## Enlaces

[Enlace a google](https://www.google.com "Google")

<https://www.google.com>

## Imagenes

![Logo de google](https://www.google.com/images/branding/googlelogo/1x/googlelogo_color_272x92dp.png "Logo de google")

## Codigo

    Puedes insertar codigo con 4 espacios al inicio de cada linea.
    Hola mundo!

~~~java
public class HolaMundo {
    public static void main(String[] args) {
        System.out.println("Hola mundo!");
    }
}
~~~
