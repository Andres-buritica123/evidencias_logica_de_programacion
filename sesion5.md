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

2.

```java

import java.util.Scanner;

public class Github {

    public static void main(String[] args) {
        System.out.println("contador de caracteres: ");
        Scanner sc = new Scanner(System.in);
        System.out.println("Ingrese cualquier texto con numeros: ");
        String cadena = sc.nextLine();
        int n1 = 0;
        int contador = 0;
        while (n1 < cadena.length()) {
            char caracter = cadena.charAt(n1);
            if (caracter == '0' || caracter == '1' || caracter == '2' || caracter == '3' || caracter == '4' || caracter == '5'
                    || caracter == '6' || caracter == '7' || caracter == '8' || caracter == '9') {
                contador++;
            }
            n1++;
        }
        System.out.println("El texto contiene " + contador + " numeros");
        sc.close();
    }
}

```

### Ejercicios - do while

1. 

```java

import java.util.Scanner;

public class Github {

    public static void main(String[] args) {
        System.out.println("contador de numeros del 1 al 100: ");
        Scanner sc = new Scanner(System.in);
        int n1; 
        do {
            System.out.println("Ingrese un numero positivo (negativo para acabar el proceso): ");
            n1 = sc.nextInt();
            while (n1 >= 0 && n1 < 100) {
                n1++;
                System.out.println(n1);
            }
        } while (n1 >= 0);
        System.out.println("Cerrando el programa....");
        sc.close();
    }

}

```

2.

```java

import java.util.Scanner;

public class Github {

    public static void main(String[] args) {
        System.out.println("Tablas de multiplicar: ");
        Scanner sc = new Scanner(System.in);
        int n1;
        int n2 = 1;
        do {
            System.out.println("Ingrese un numero entero (0 para acabar el programa): ");
            n1 = sc.nextInt();
            if (n1 != 0) {
                System.out.println("Tabla de multiplicar del " + n1 + ": ");
                while (n2 <= 12) {
                    int resp = n1 * n2;
                    System.out.println(n1 + "*" + n2 + "=" + resp);
                    n2++;
                }
                n2 = 1;
            }
        } while (n1 != 0);
        System.out.println("Cerrando el programa");
        sc.close();
    }

}

```

### Ejercicios - for

1. 

```java

public class Github {

    public static void main(String[] args) {
        System.out.println("Numeros impares del 1 al 50: ");
        for (int n1 = 1; n1 <= 50; n1 += 2){
            System.out.println(n1);
        }
    }

}

```

2.

```java

public class Github {

    public static void main(String[] args) {
        boolean n_primos;
        System.out.println("Numero primos del 1 al 100: ");
        for (int n1 = 2; n1 <= 100; n1++) {
            n_primos = true;
            for (int n2 = n1 - 1; n2 > 1; n2--) {
                if (n1 % n2 == 0) {
                    n_primos = false;
                    break;
                }

            }
            if (n_primos) {
                System.out.println(n1);
            }
        }
    }

}

```
