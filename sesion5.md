<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 5 

## Actividad 5: Ejercicios de bucles

Resolver los siguientes ejercicios:

### Ejercicios - while

1. Pedir al usuario que ingrese un número y mostrar su tabla de multiplicar hasta el número 10.

2. Pedir al usuario que ingrese una cadena de caracteres y contar la cantidad de caracteres que son números.

### Ejercicios - do while

1. Escribe un programa en Java que imprima los números del 1 al 100, pero que se detenga si el usuario introduce un número negativo.

2. Escribe un programa en Java que pida al usuario un número entero e imprima la tabla de multiplicar de ese número, pero que se detenga si el usuario introduce el número 0.

### Ejercicios - for

1. Imprimir los números impares del 1 al 50.

2. Imprimir los números primos del 1 al 100.

## Solución actividad 5

### Ejercicios - while

1. 

```java

import java.util.Scanner;

public class Github {

    public static void main(String[] args) {
        System.out.println("Tabla de multiplicar hasta el 10 de cualquier numero: ");
        Scanner sc = new Scanner(System.in);
        System.out.println("Ingrese un numero entero: ");
        int n1 = sc.nextInt();
        int n2 = 1;
        System.out.println("Tabla de multiplicar hasta el 10 del numero " + n1 + ": ");
        while (n2 <= 10) {
            int resp = n1 * n2;

            System.out.println(n1 + "*" + n2 + "=" + resp);
            n2++;
        }
        sc.close();
    }
}

```

### Ejercicios - do while

### Ejercicios - for