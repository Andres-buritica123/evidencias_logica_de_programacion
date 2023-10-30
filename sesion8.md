<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 8 

## Actividad: Ejecicios de métodos en Java
Implementar los siguientes métodos:

1. Escribe un método que reciba dos números como parámetros y devuelva el mayor de los dos.

2. Escribe un método que reciba una cadena de texto como parámetro y devuelva el número de vocales que contiene.

3. Escribe un método que reciba una cadena de texto como parámetro y devuelva una nueva cadena con todas las letras mayúsculas en minúsculas y viceversa.

4. Escribe un método que reciba una cadena de texto como parámetro y devuelva el número de palabras que contiene.

5. Escribe un método que reciba una cadena de texto como parámetro y devuelva una nueva cadena con todas las palabras en orden alfabético.

## Solución actividad 8

1. 

```java

import java.util.Scanner;

public class Github {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n1, n2;
        System.out.println("Ingrese el primer numero: ");
        n1 = sc.nextInt();
        System.out.println("Ingrese el segundo numero: ");
        n2 = sc.nextInt();
        String resp = numeromayor(n1, n2);
        System.out.println(resp);
        sc.close();
    }

    public static String numeromayor(int a, int b) {
        if (a > b) {
            return "El primer numero es mayor que el segundo";
        } else if (b > a) {
            return "El segundo numero es mayor que el primero";
        } else {
            return "Los numeros son iguales";
        }
    }
}

```

2. 

```java

import java.util.Scanner;

public class Github {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Ingrese una cadena de caracteres: ");
        String cadena = sc.nextLine();
        int contador2 = contador(cadena);
        System.out.println("La cadena ingresada contiene " + contador2 + " vocales.");
        sc.close();
    }

    public static int contador(String cadena) {
        int i = 0;
        int contadorVocales = 0;
        while (i < cadena.length()) {
            char caracter = cadena.charAt(i);
            if (caracter == 'a' || caracter == 'e' || caracter == 'i' || caracter == 'o' || caracter == 'u'
                    || caracter == 'A' || caracter == 'E' || caracter == 'I' || caracter == 'O' || caracter == 'U') {
                contadorVocales++;
            }
            i++;
        }
        return contadorVocales;
    }
}

```

3. 

```java

import java.util.Scanner;

public class Github {

    public static void main(String[] args) {
        Scanner sc = new Scanner (System.in);
        System.out.println("Ingrese un cadeda de texto");
        String cd1 = sc.nextLine();
        mayor(cd1);
        sc.close();
    }
    public static String mayor (String cd1){
        String c1 = cd1.toUpperCase();
        System.out.println("Cadena ingresada transformada a mayusculas");
        System.out.println(c1);
        String c2 = cd1.toLowerCase();
        System.out.println("Cadena ingresada transformada a minusculas");
        System.out.println(c2);
        return cd1;

    }
}
 
 ```

 4. 

 ```java

 