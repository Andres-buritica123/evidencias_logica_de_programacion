<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 7 

## Actividad: Ejecicios Array - ArrayList

### 1. En parejas, probar, analizar y explicar el funcionamiento de los siguientes ejemplos de Array y ArrayList.

+ Ejemplo Array

```java

import java.util.Arrays;

public class EjercicioArray {

    public static void main(String[] args) {
        // Crear un array de números enteros
        int[] numeros = {5, 2, 10, 7, 1};

        // Imprimir el array original
        System.out.println("Array original: " + Arrays.toString(numeros));

        // Calcular la suma de los elementos del array
        int suma = 0;
        for (int i = 0; i < numeros.length; i++) {
            suma += numeros[i];
        }
        System.out.println("La suma de los elementos es: " + suma);

        // Encontrar el número más grande en el array
        int maximo = numeros[0];
        for (int i = 1; i < numeros.length; i++) {
            if (numeros[i] > maximo) {
                maximo = numeros[i];
            }
        }
        System.out.println("El número más grande es: " + maximo);

        // Ordenar el array en orden ascendente
        Arrays.sort(numeros);
        System.out.println("Array ordenado: " + Arrays.toString(numeros));
    }
}

```

+ Ejemplo Array list

```java

import java.util.ArrayList; 
import java.util.Scanner;

public class AppNotas {

  public static void main(String[] args) {

    ArrayList<String> notas = new ArrayList<>();
    
    Scanner scan = new Scanner(System.in);

    while(true) {

      System.out.println("1. Agregar nota");  
      System.out.println("2. Mostrar notas");
      System.out.println("3. Salir");

      int opcion = scan.nextInt();

      if (opcion == 1) {
        agregarNota(notas, scan);  
      } else if (opcion == 2) {
        mostrarNotas(notas);
      } else {
        break;
      }

    }

  }

  public static void agregarNota(ArrayList<String> notas, Scanner scan) {
    
    System.out.println("Ingrese el titulo de la nota:");
    String titulo = scan.nextLine();
    
    System.out.println("Ingrese el contenido de la nota:");
    String contenido = scan.nextLine();
    
    notas.add(titulo + " - " + contenido);

  }

  public static void mostrarNotas(ArrayList<String> notas) {

    for(String n : notas) {
      System.out.println(n);
    }

  }

}

```

### 2. Crear un ejemplo de Array y otro de ArrayList para visualizar sus diferencias.

## Solución actividad 7

1. Array

```java

public class Github {

    public static void main(String[] args) {
        String bmw = "BMW";
        String ford = "Ford";
        String lamboghini = "Lamboghini";
        String mazda = "Mazda";
        String tesla = "Tesla Inc";
        String ferrari = "Ferrari";
        String toyota = "Toyota";
        String volkswagen = "Volkswagen";
        String porsche = "Porsche";
        
        String[] numeros = new String[10];
        numeros[1] = bmw;
        numeros[2] = ford;
        numeros[3] = lamboghini;
        numeros[4] = mazda;
        numeros[5] = tesla;
        numeros[6] = ferrari;
        numeros[7] = toyota;
        numeros[8] = volkswagen;
        numeros[9] = porsche;

        System.out.println("Que marca de carro le gusta más y si es buena elección");
        System.out.println("""
                           1 = BMW
                           2 = Ford
                           3 = Lamboghini
                           4 = Mazda
                           5 = Tesla Inc
                           6 = Ferrari  
                           7 = Toyota
                           8 = Volkswagen
                           9 = Porsche""");
        String carro = numeros[9];
        System.out.println("Marca de carro elgida: " + carro + "; es buena elección");
    }

}


```

2. ArrayList

```java

import java.util.ArrayList;


public class Github {

    public static void main(String[] args) {

        ArrayList<String> nombreArrayList = new ArrayList<>();
        
        for (int i = 1; i <= 10; i++) {
            nombreArrayList.add("Elemento " + i);
        }
        nombreArrayList.add(0, "Elemento 3");

        for (String elemento : nombreArrayList) {
            System.out.print(elemento + " / ");
        }
    }
}

```
