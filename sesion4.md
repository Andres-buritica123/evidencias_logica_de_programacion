<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 4

## Actividad 4: Ejercicios de control de flujo con expresiones compuestas

```java

// Variables de tipo String
String nombre = "Juan Pérez";
String apellido = "González";
String identificación = "1000000001";
String correo = "juan.perez@ejemplo.com";
String carrera = "Desarrollo de Software";
String universidad = "Cesde";
// Variable de tipo int
int edad = 20;
// Variable de tipo boolean
boolean esActivo = true;
boolean becado = false;
// Variable de tipo char
char género = 'M';
// Variable de tipo double
double promedio = 4.5;
// Variable de tipo int
int semestre = 2;

```
- Con la información anterior, implementa los siguientes ejercicios:

1. Determinar si el estudiante es mayor de edad y tiene un estado activo.

2. Determinar si el estudiante tiene una beca o una carrera relacionada con el desarrollo de software.

3. Determinar si el estudiante está en el último semestre de su carrera y tiene un estado activo.

4. Determinar si el estudiante tiene una carrera relacionada con el desarrollo de software y un promedio superior a 4.0.

5. Mostrar toda la información del estudiante si está matriculado en el Cesde.

6. Asignar una beca del 50% si el estudiante está matriculado en el Cesde, tiene un promedio superior a 4.0 y está activo.

7. Determinar la cantidad de beca que recibe el estudiante según su promedio:
   - 0.0 - 3.4: El estudiante no recibe beca.
   - 3.5 - 3.9: El estudiante recibe una beca parcial del 25%.
   - 4.0 - 4.4: El estudiante recibe una beca parcial del 50%.
   - 4.5 - 5.0: El estudiante recibe una beca completa.

## Solucion actividad 4

```java

public class Github {

    public static void main(String[] args) {
        String nombre = "Juan Pérez";
        String apellido = "González";
        String identificación = "1000000001";
        String correo = "juan.perez@ejemplo.com";
        String carrera = "Desarrollo de Software";
        String universidad = "Cesde";
        int edad = 20;
        boolean esActivo = true;
        boolean becado = false;
        char género = 'M';
        double promedio = 4.5;
        int semestre = 2;

        System.out.println("Ejercicio 1: ");
        if (edad >= 18 && esActivo) {
            System.out.println("El estudiante es mayor de edad y esta activo");
        }
        
        System.out.println("Ejercicio 2: ");
        if (!becado && carrera.equals("Desarrollo de Software")) {
            System.out.println("El estudiante es becado y estudia desarrollo de software");
        }
        
        System.out.println("Ejercicio 3: ");
        if (semestre == 2 && esActivo) {
            System.out.println("El estudiante esta en el semestre 2 y tiene estado activo");
        }
        
        System.out.println("Ejercicio 4: ");
        if (carrera.equals("Desarrollo de Software") && promedio > 4.0) {
            System.out.println("Si estudia desarrollo de software y si tiene promedio superior a 4.0");
        }
        
        System.out.println("Esjecicio 5: ");
        if (universidad.equals("Cesde")) {
            System.out.println("Es estudiante del CESDE");
            System.out.println("Informacion del estudiante: ");
            System.out.println("Nombre: " + nombre);
            System.out.println("Apellido: " + apellido);
            System.out.println("Identificación: " + identificación);
            System.out.println("Correo: " + correo);
            System.out.println("Estudia: " + carrera);
            System.out.println("Universidad: " + universidad);
            System.out.println("Edad: " + edad);
            System.out.println("Tiene un estado activo: " + esActivo);
            System.out.println("Es becado: " + becado);
            System.out.println("Género: " + género);
            System.out.println("Promedio: " + promedio);
            System.out.println("Semestre en el que va: " + semestre);
        }
        
        System.out.println("Ejercicio 6: ");
        if (universidad.equals("Cesde") && promedio > 4.0 && esActivo) {
            System.out.println("Obtienes una beca de 50%");
        }
        
        System.out.println("Ejercicio 7: ");
        if (promedio >= 4.5) {
            System.out.println("Obtienes una beca completa");
        }
    }
}

```
