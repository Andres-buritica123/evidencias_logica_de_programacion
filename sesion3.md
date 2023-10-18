<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 3 

## Actividad 3: Ejercicios de operaciones básicas en Java.

1. Suma y multiplicación: Escribe un programa que solicite al usuario dos números enteros y luego imprima la suma y multiplicación de esos números.[^1].

2. Resta y división: Escribe un programa que tome dos números enteros ingresados por el usuario y calcule la resta y división de esos números.[^2].

3. Operaciones combinadas: Escribe un programa que solicite al usuario tres números enteros y realice las siguientes operaciones: suma de los tres números, multiplicación del primer número por el segundo y división del resultado entre el tercer número.[^3].

4. Operaciones con decimales: Escribe un programa que solicite al usuario dos números decimales y realice las siguientes operaciones: suma, resta, multiplicación y división.[^4].

5. Incremento y decremento: Escribe un programa que declare una variable entera y la inicialice con un valor. Luego, incrementa su valor en 1 y muestra el resultado. Después, decrementa su valor en 1 y muestra el resultado nuevamente.[^5].

6. Operador de asignación compuesta: Escribe un programa que declare una variable entera y la inicialice con un valor. Utiliza el operador de asignación compuesta para sumar 5 a la variable y luego mostrar su valor.[^6].

7. Operadores lógicos: Escribe un programa que tome dos valores booleanos ingresados por el usuario y muestre el resultado de las operaciones lógicas AND, OR y NOT entre esos valores.[^7].

8. Operador ternario: Escribe un programa que tome un número entero ingresado por el usuario y utilice el operador ternario para determinar si el número es positivo o negativo. Luego, muestra el resultado en la salida.[^8].

## Solución actividad 3

[^1]: Suma y multiplicación:

```java

import java.util.Scanner;

public class Github {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("Suma y multiplicación de numeros enteros: ");
        System.out.println("Ingrese un numero entero: ");
        int n1 = sc.nextInt();
        System.out.println("Ingrese el segundo numero entero: ");
        int n2 = sc.nextInt();
        int suma = n1 + n2;
        int mul = n1 * n2;
        System.out.println("El resultado de la suma es: " + suma);
        System.out.println("El resultado de la multiplicación es: " + mul);
        sc.close();
    }
}

```

[^2]: Resta y division:

```java

import java.util.Scanner;

public class Github {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("Resta y divición de numeros enteros: ");
        System.out.println("Ingrese un numero entero: ");
        int n1 = sc.nextInt();
        System.out.println("Ingrese el segundo numero entero: ");
        int n2 = sc.nextInt();
        int resta = n1 - n2;
        int div = n1 / n2;
        System.out.println("El resultado de la resta es: " + resta);
        System.out.println("El resultado de la divición es: " + div);
        sc.close();
    }
}

```
[^3]: Operaciones combinadas:

```java

import java.util.Scanner;

public class Github {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("Operaciones combinadas de numeros enteros: ");
        System.out.println("Ingrese un numero entero: ");
        int n1 = sc.nextInt();
        System.out.println("Ingrese el segundo numero entero: ");
        int n2 = sc.nextInt();
        System.out.println("Ingrese el tercer numero entero: ");
        int n3 = sc.nextInt();
        int suma = n1 + n2 + n3;
        int mul = n1 * n2;
        int div = mul / n3;
        System.out.println("El resultado de la suma es: " + suma);
        System.out.println("El resultado de la multiplicación es: " + mul);
        System.out.println("El resultado de la divición es: " + div);
        sc.close();
    }
}

```

[^4]: Operaciones con dcimales:

```java

import java.util.Scanner;

public class Github {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("Operaciones con numeros decimales: ");
        System.out.println("Ingrese un numero decimal: ");
        double n1 = sc.nextDouble();
        System.out.println("Ingrese el segundo numero decimal: ");
        double n2 = sc.nextDouble();
        double suma = n1 + n2;
        double resta = n1 - n2;
        double mul = n1 * n2;
        double div = n1 / n2;
        System.out.println("El resultado de la suma es: " + suma);
        System.out.println("El resultado de la resta es: " + resta);
        System.out.println("El resultado de la multiplicación es: " + mul);
        System.out.println("El resultado de la divición es: " + div);
        sc.close();
    }
}

```

[^5]: Incremento y decremento:

```java

public class Github {

    public static void main(String[] args) {
        System.out.println("Incremento y decremento con numeros enteros: ");
        int n1 = 150;
        System.out.println("El valor de la variable es: " + n1);
        n1++;
        System.out.println("El valor de la variable incrementado en 1 es: " + n1);
        n1--;
        System.out.println("El valor de la variable decremantado en 1 es: " + n1);
    }
}

```

[^6]: Operador de asignación compuesta:

```java

public class Github {

    public static void main(String[] args) {
        System.out.println("Operador de asignación compuesta: ");
        int n1 = 150;
        n1 = n1 + 5;
        System.out.println("El resultado de la operación es: " + n1);
    }
}

```

[^7]: Operadores lógicos:

```java

import java.util.Scanner;

public class Github {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("Operadores lógicos: ");
        System.out.println("Ingrese true o false: ");
        boolean b1 = sc.nextBoolean();
        System.out.println("Ingrese false o true: ");
        boolean b2 = sc.nextBoolean();
        System.out.println("Resultado del booleano and (&&): " + (b1 && b2));
        System.out.println("Resultado del booleano or (||): " + (b1 || b2));
        System.out.println("Resultado del booleano not(!)" + (!b2));
        sc.close();
    }
}

```

[^8]: Operador ternario:

```java

import java.util.Scanner;

public class Github {

    public static void main(String[] args) {
        System.out.println("Operador ternario: ");
        Scanner sc = new Scanner(System.in);
        System.out.println("Ingrese un numero entero: ");
        int n1 = sc.nextInt();
        String resp = (n1 > 0) ? "positivo" : "negativo";
        System.out.println("El numero es: " + resp);
        sc.close();
    }
}

```
