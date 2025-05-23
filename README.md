# Taller-POO-y-UML

Sección 1: Sintaxis y Tipos Primitivos (com.taller.seccion1)

// Ejercicio 1: Declaración de variables de diferentes tipos
package com.taller.seccion1;

public class Ejercicio1 {
    public static void main(String[] args) {
        // Declaración de variables de distintos tipos
        int edad = 25;
        double salario = 1500.50;
        char genero = 'M';
        String nombre = "Juan Pérez";
        boolean esEstudiante = true;
        
        // Impresión de las variables
        System.out.println("Edad: " + edad);
        System.out.println("Salario: " + salario);
        System.out.println("Género: " + genero);
        System.out.println("Nombre: " + nombre);
        System.out.println("¿Es estudiante?: " + esEstudiante);
    }
}

// Ejercicio 2: Impresión de variables
package com.taller.seccion1;

public class Ejercicio2 {
    public static void main(String[] args) {
        // Declaración e inicialización de variables
        int numEntero = 42;
        double numDecimal = 3.14159;
        char caracter = 'A';
        String texto = "Hola Mundo";
        boolean condicion = false;
        
        // Impresión utilizando System.out.println
        System.out.println("Valor entero: " + numEntero);
        System.out.println("Valor decimal: " + numDecimal);
        System.out.println("Carácter: " + caracter);
        System.out.println("Texto: " + texto);
        System.out.println("Condición: " + condicion);
    }
}

// Ejercicio 3: Operadores aritméticos
package com.taller.seccion1;

public class Ejercicio3 {
    public static void main(String[] args) {
        // Declaración de variables
        int a = 15;
        int b = 4;
        
        // Operadores aritméticos
        int suma = a + b;
        int resta = a - b;
        int multiplicacion = a * b;
        int division = a / b;
        int modulo = a % b;
        
        // Mostrar resultados
        System.out.println("Suma: " + a + " + " + b + " = " + suma);
        System.out.println("Resta: " + a + " - " + b + " = " + resta);
        System.out.println("Multiplicación: " + a + " * " + b + " = " + multiplicacion);
        System.out.println("División: " + a + " / " + b + " = " + division);
        System.out.println("Módulo: " + a + " % " + b + " = " + modulo);
    }
}

// Ejercicio 4: Operadores relacionales y lógicos
package com.taller.seccion1;

public class Ejercicio4 {
    public static void main(String[] args) {
        int x = 10;
        int y = 20;
        boolean p = true;
        boolean q = false;
        
        // Operadores relacionales
        System.out.println("x < y: " + (x < y));
        System.out.println("x > y: " + (x > y));
        System.out.println("x == y: " + (x == y));
        System.out.println("x != y: " + (x != y));
        
        // Operadores lógicos
        System.out.println("p && q: " + (p && q));
        System.out.println("p || q: " + (p || q));
        System.out.println("!p: " + (!p));
    }
}

// Ejercicio 5: Comentarios
package com.taller.seccion1;

public class Ejercicio5 {
    public static void main(String[] args) {
        // Este es un comentario de una línea
        
        /*
         * Este es un comentario
         * de múltiples líneas
         * que explica el propósito del código
         */
        
        int x = 5; // Comentario al final de una línea
        
        // Calculamos el cuadrado del número
        int cuadrado = x * x;
        
        /* El siguiente código muestra el resultado
         * del cálculo anterior
         */
        System.out.println("El cuadrado de " + x + " es: " + cuadrado);
    }
}

// Ejercicio 6: Lectura de datos con Scanner
package com.taller.seccion1;

import java.util.Scanner;

public class Ejercicio6 {
    public static void main(String[] args) {
        // Crear un objeto Scanner para leer entrada del usuario
        Scanner scanner = new Scanner(System.in);
        
        // Solicitar y leer un entero
        System.out.print("Ingrese un número entero: ");
        int entero = scanner.nextInt();
        
        // Solicitar y leer un número decimal
        System.out.print("Ingrese un número decimal: ");
        double decimal = scanner.nextDouble();
        
        // Mostrar los valores ingresados
        System.out.println("Número entero ingresado: " + entero);
        System.out.println("Número decimal ingresado: " + decimal);
        
        // Cerrar el scanner para liberar recursos
        scanner.close();
    }
}

// Ejercicio 7: Conversión de tipos
package com.taller.seccion1;

public class Ejercicio7 {
    public static void main(String[] args) {
        // Convertir String a tipos numéricos
        String numeroStr = "123";
        
        int numeroInt = Integer.parseInt(numeroStr);
        double numeroDouble = Double.parseDouble(numeroStr);
        
        System.out.println("String a int: " + numeroInt);
        System.out.println("String a double: " + numeroDouble);
        
        // Convertir tipos numéricos a String
        int valor1 = 456;
        double valor2 = 789.12;
        
        String valorStr1 = Integer.toString(valor1);
        String valorStr2 = Double.toString(valor2);
        
        System.out.println("int a String: " + valorStr1);
        System.out.println("double a String: " + valorStr2);
    }
}

// Ejercicio 8: Manejo de excepciones
package com.taller.seccion1;

public class Ejercicio8 {
    public static void main(String[] args) {
        String valorCorrecto = "123";
        String valorIncorrecto = "abc";
        
        // Convertir un String válido a entero
        try {
            int numero1 = Integer.parseInt(valorCorrecto);
            System.out.println("Conversión exitosa: " + numero1);
        } catch (NumberFormatException e) {
            System.out.println("Error al convertir: " + valorCorrecto);
        }
        
        // Convertir un String inválido a entero
        try {
            int numero2 = Integer.parseInt(valorIncorrecto);
            System.out.println("Conversión exitosa: " + numero2);
        } catch (NumberFormatException e) {
            System.out.println("Error al convertir: '" + valorIncorrecto + "' no es un número válido");
            System.out.println("Mensaje de error: " + e.getMessage());
        }
    }
}

// Ejercicio 9: Constantes con final
package com.taller.seccion1;

public class Ejercicio9 {
    public static void main(String[] args) {
        // Declaración de constantes
        final double PI = 3.14159;
        final String NOMBRE_EMPRESA = "MiEmpresa S.A.";
        final int DIAS_SEMANA = 7;
        
        // Uso de las constantes
        double radio = 5.0;
        double area = PI * radio * radio;
        
        System.out.println("Valor de PI: " + PI);
        System.out.println("Nombre de la empresa: " + NOMBRE_EMPRESA);
        System.out.println("Días de la semana: " + DIAS_SEMANA);
        System.out.println("Área del círculo con radio " + radio + ": " + area);
        
        // No se puede modificar una constante
        // PI = 3.14; // Esto generaría un error de compilación
    }
}

// Ejercicio 10: Uso de la clase Math
package com.taller.seccion1;

public class Ejercicio10 {
    public static void main(String[] args) {
        double base = 2.0;
        double exponente = 3.0;
        double numero = 25.0;
        
        // Cálculo de potencia
        double potencia = Math.pow(base, exponente);
        System.out.println(base + " elevado a " + exponente + " = " + potencia);
        
        // Cálculo de raíz cuadrada
        double raizCuadrada = Math.sqrt(numero);
        System.out.println("La raíz cuadrada de " + numero + " = " + raizCuadrada);
        
        // Otros métodos de Math
        System.out.println("Valor absoluto de -10: " + Math.abs(-10));
        System.out.println("Redondeo de 3.75: " + Math.round(3.75));
        System.out.println("Máximo entre 8 y 12: " + Math.max(8, 12));
    }
}

// Ejercicio 11: Número aleatorio con Math.random()
package com.taller.seccion1;

public class Ejercicio11 {
    public static void main(String[] args) {
        // Generar número aleatorio entre 0.0 (inclusive) y 1.0 (exclusive)
        double numeroAleatorio = Math.random();
        System.out.println("Número aleatorio entre 0 y 1: " + numeroAleatorio);
        
        // Generar número aleatorio entre 1 y 100
        int min = 1;
        int max = 100;
        int aleatorioEntero = (int)(Math.random() * (max - min + 1)) + min;
        System.out.println("Número aleatorio entre " + min + " y " + max + ": " + aleatorioEntero);
        
        // Generar 5 números aleatorios adicionales entre 1 y 10
        System.out.println("Cinco números aleatorios entre 1 y 10:");
        for (int i = 0; i < 5; i++) {
            int numero = (int)(Math.random() * 10) + 1;
            System.out.println("Número " + (i+1) + ": " + numero);
        }
    }
}

// Ejercicio 12: Formateo de salida
package com.taller.seccion1;

public class Ejercicio12 {
    public static void main(String[] args) {
        String nombre = "Ana";
        int edad = 28;
        double salario = 1234.56789;
        
        // Formateo con System.out.printf
        System.out.printf("Nombre: %s, Edad: %d años\n", nombre, edad);
        
        // Formateo de números decimales
        System.out.printf("Salario con 2 decimales: %.2f\n", salario);
        System.out.printf("Salario con formato monetario: $%,.2f\n", salario);
        
        // Alineación y ancho de campo
        System.out.printf("%-10s | %5d | %10.2f\n", "Nombre", "Edad", "Salario");
        System.out.printf("%-10s | %5d | %10.2f\n", nombre, edad, salario);
        
        // Formateo de fechas y porcentajes
        System.out.printf("Porcentaje: %.1f%%\n", 85.5);
    }
}

// Ejercicio 13: Código ASCII
package com.taller.seccion1;

import java.util.Scanner;

public class Ejercicio13 {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        System.out.print("Ingrese un carácter: ");
        char caracter = scanner.next().charAt(0);
        
        // Convertir char a su código ASCII (implícitamente se convierte a int)
        int codigoAscii = caracter;
        
        System.out.println("El carácter '" + caracter + "' tiene el código ASCII: " + codigoAscii);
        
        // Mostrar información adicional
        if (codigoAscii >= 65 && codigoAscii <= 90) {
            System.out.println("Es una letra mayúscula.");
        } else if (codigoAscii >= 97 && codigoAscii <= 122) {
            System.out.println("Es una letra minúscula.");
        } else if (codigoAscii >= 48 && codigoAscii <= 57) {
            System.out.println("Es un dígito numérico.");
        } else {
            System.out.println("Es un carácter especial.");
        }
        
        scanner.close();
    }
}

// Ejercicio 14: Verificar si un String está vacío
package com.taller.seccion1;

public class Ejercicio14 {
    public static void main(String[] args) {
        String texto1 = "Hola Mundo";
        String texto2 = "";
        String texto3 = "   ";
        String texto4 = null;
        
        // Verificar si texto1 está vacío
        boolean esVacio1 = texto1.isEmpty();
        System.out.println("¿'" + texto1 + "' está vacío? " + esVacio1);
        
        // Verificar si texto2 está vacío
        boolean esVacio2 = texto2.isEmpty();
        System.out.println("¿'" + texto2 + "' está vacío? " + esVacio2);
        
        // Verificar si texto3 está vacío (contiene solo espacios)
        boolean esVacio3 = texto3.isEmpty();
        System.out.println("¿'" + texto3 + "' está vacío? " + esVacio3);
        
        // Verificar si texto3 está vacío después de eliminar espacios
        boolean esVacio3Trim = texto3.trim().isEmpty();
        System.out.println("¿'" + texto3 + "' está vacío después de trim? " + esVacio3Trim);
        
        // Verificar texto4 (null) con manejo de excepciones
        try {
            boolean esVacio4 = texto4.isEmpty();
            System.out.println("¿'" + texto4 + "' está vacío? " + esVacio4);
        } catch (NullPointerException e) {
            System.out.println("No se puede verificar si texto4 está vacío porque es null");
        }
    }
}

// Ejercicio 15: Reflexión sobre tipos primitivos vs objetos
package com.taller.seccion1;

public class Ejercicio15 {
    public static void main(String[] args) {
        // Tipos primitivos
        int numeroInt = 10;
        double numeroDouble = 20.5;
        boolean condicion = true;
        
        // Objetos (Wrappers)
        Integer numeroIntegerObj = 10;
        Double numeroDoubleObj = 20.5;
        Boolean condicionObj = true;
        String textoObj = "Hola";
        
        // Demostración de diferencias
        System.out.println("---- Tipos Primitivos ----");
        System.out.println("int: " + numeroInt);
        System.out.println("double: " + numeroDouble);
        System.out.println("boolean: " + condicion);
        
        System.out.println("\n---- Objetos ----");
        System.out.println("Integer: " + numeroIntegerObj);
        System.out.println("Double: " + numeroDoubleObj);
        System.out.println("Boolean: " + condicionObj);
        System.out.println("String: " + textoObj);
        
        // Demostración de métodos disponibles solo en objetos
        System.out.println("\n---- Métodos de objetos ----");
        System.out.println("Integer.toString(): " + numeroIntegerObj.toString());
        System.out.println("Double.intValue(): " + numeroDoubleObj.intValue());
        System.out.println("Boolean.compareTo(): " + condicionObj.compareTo(false));
        System.out.println("String.length(): " + textoObj.length());
        
        // Valores null (solo posible en objetos)
        Integer nulo = null;
        System.out.println("\n---- Valores null ----");
        System.out.println("Objeto con valor null: " + nulo);
        // int nuloPrimitivo = null; // Esto generaría un error de compilación
    }
}

Sección 2: Estructuras de Control (com.taller.seccion2)

// Ejercicio 1: Implementa if simple y if-else
package com.taller.seccion2;

import java.util.Scanner;

public class Ejercicio1 {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        // if simple
        System.out.print("Ingrese su edad: ");
        int edad = scanner.nextInt();
        
        if (edad >= 18) {
            System.out.println("Eres mayor de edad.");
        }
        
        // if-else
        System.out.print("Ingrese la temperatura actual (°C): ");
        double temperatura = scanner.nextDouble();
        
        if (temperatura > 25) {
            System.out.println("Hace calor.");
        } else {
            System.out.println("No hace calor.");
        }
        
        scanner.close();
    }
}

// Ejercicio 2: Usa if-else if-else para categorizar edades
package com.taller.seccion2;

import java.util.Scanner;

public class Ejercicio2 {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        System.out.print("Ingrese su edad: ");
        int edad = scanner.nextInt();
        
        // Categorización de edades usando if-else if-else
        if (edad < 0) {
            System.out.println("La edad no puede ser negativa.");
        } else if (edad < 12) {
            System.out.println("Eres un niño.");
        } else if (edad < 18) {
            System.out.println("Eres un adolescente.");
        } else if (edad < 65) {
            System.out.println("Eres un adulto.");
        } else {
            System.out.println("Eres un anciano.");
        }
        
        scanner.close();
    }
}

// Ejercicio 3: Implementa switch para opciones de menú numérico
package com.taller.seccion2;

import java.util.Scanner;

public class Ejercicio3 {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        System.out.println("===== MENÚ DE OPCIONES =====");
        System.out.println("1. Ver saldo");
        System.out.println("2. Depositar dinero");
        System.out.println("3. Retirar dinero");
        System.out.println("4. Ver últimos movimientos");
        System.out.println("5. Salir");
        System.out.print("Seleccione una opción (1-5): ");
        
        int opcion = scanner.nextInt();
        
        // Menú con switch
        switch (opcion) {
            case 1:
                System.out.println("Saldo actual: $1000.00");
                break;
            case 2:
                System.out.println("Operación de depósito seleccionada.");
                break;
            case 3:
                System.out.println("Operación de retiro seleccionada.");
                break;
            case 4:
                System.out.println("Mostrando últimos movimientos...");
                break;
            case 5:
                System.out.println("Gracias por utilizar nuestro servicio. ¡Hasta pronto!");
                break;
            default:
                System.out.println("Opción no válida. Por favor seleccione una opción del 1 al 5.");
        }
        
        scanner.close();
    }
}

// Ejercicio 4: Crea bucle for para imprimir 1-20 y su factorial
package com.taller.seccion2;

public class Ejercicio4 {
    public static void main(String[] args) {
        System.out.println("Número\tFactorial");
        System.out.println("-------------------");
        
        // Bucle for para calcular e imprimir factoriales del 1 al 20
        for (int i = 1; i <= 20; i++) {
            // Cálculo del factorial
            long factorial = 1;
            for (int j = 1; j <= i; j++) {
                factorial *= j;
            }
            
            // Impresión del número y su factorial
            System.out.println(i + "\t" + factorial);
        }
    }
}

// Ejercicio 5: Crea bucle while que sume números hasta que el usuario ingrese 0
package com.taller.seccion2;

import java.util.Scanner;

public class Ejercicio5 {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        int numero;
        int suma = 0;
        int contador = 0;
        
        System.out.println("Ingrese números para sumar (0 para terminar):");
        
        // Bucle while para sumar números hasta que se ingrese 0
        while ((numero = scanner.nextInt()) != 0) {
            suma += numero;
            contador++;
            System.out.println("Suma actual: " + suma);
        }
        
        System.out.println("Suma total: " + suma);
        System.out.println("Cantidad de números ingresados: " + contador);
        
        if (contador > 0) {
            double promedio = (double) suma / contador;
            System.out.println("Promedio: " + promedio);
        }
        
        scanner.close();
    }
}

// Ejercicio 6: Crea bucle do-while para pedir contraseña hasta ser correcta
package com.taller.seccion2;

import java.util.Scanner;

public class Ejercicio6 {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        final String PASSWORD_CORRECTA = "java123";
        String passwordIngresada;
        int intentos = 0;
        
        do {
            intentos++;
            System.out.print("Ingrese la contraseña (intento " + intentos + "): ");
            passwordIngresada = scanner.nextLine();
            
            if (passwordIngresada.equals(PASSWORD_CORRECTA)) {
                System.out.println("¡Contraseña correcta! Acceso concedido.");
            } else {
                System.out.println("Contraseña incorrecta. Intente nuevamente.");
            }
            
        } while (!passwordIngresada.equals(PASSWORD_CORRECTA) && intentos < 3);
        
        if (!passwordIngresada.equals(PASSWORD_CORRECTA)) {
            System.out.println("Ha alcanzado el número máximo de intentos. Acceso denegado.");
        }
        
        scanner.close();
    }
}

// Ejercicio 7: Rompe bucles con break y continúa con continue
package com.taller.seccion2;

public class Ejercicio7 {
    public static void main(String[] args) {
        System.out.println("Ejemplo de break:");
        // Uso de break para salir de un bucle
        for (int i = 1; i <= 10; i++) {
            if (i == 6) {
                System.out.println("Encontrado el valor 6, saliendo del bucle con break.");
                break; // Sale del bucle cuando i es 6
            }
            System.out.println("Valor de i: " + i);
        }
        
        System.out.println("\nEjemplo de continue:");
        // Uso de continue para saltar iteraciones
        for (int i = 1; i <= 10; i++) {
            if (i % 2 == 0) {
                System.out.println("Encontrado valor par " + i + ", saltando con continue.");
                continue; // Salta el resto de la iteración cuando i es par
            }
            System.out.println("Procesando valor impar: " + i);
        }
    }
}

// Ejercicio 8: Anida bucles para imprimir tabla de multiplicar (1-10)
package com.taller.seccion2;

public class Ejercicio8 {
    public static void main(String[] args) {
        System.out.println("TABLA DE MULTIPLICAR (1-10)");
        
        // Imprimir encabezado
        System.out.print("   | ");
        for (int i = 1; i <= 10; i++) {
            System.out.printf("%4d", i);
        }
        System.out.println("\n---+----------------------------------------");
        
        // Anidación de bucles para tabla de multiplicar
        for (int i = 1; i <= 10; i++) {
            System.out.printf("%2d | ", i);
            
            for (int j = 1; j <= 10; j++) {
                System.out.printf("%4d", i * j);
            }
            
            System.out.println();
        }
    }
}

// Ejercicio 9: Usa for-each para recorrer un array de String
package com.taller.seccion2;

public class Ejercicio9 {
    public static void main(String[] args) {
        // Declaración e inicialización de un array de String
        String[] frutas = {"Manzana", "Banana", "Cereza", "Durazno", "Fresa", "Kiwi", "Mango"};
        
        System.out.println("Lista de frutas:");
        
        // Recorrido del array usando for-each
        for (String fruta : frutas) {
            System.out.println("- " + fruta);
        }
        
        // Contando caracteres en cada fruta
        System.out.println("\nNombre y cantidad de letras:");
        
        for (String fruta : frutas) {
            System.out.println(fruta + ": " + fruta.length() + " letras");
        }
    }
}

Ejercicio 10: Implementar recursión para calcular Fibonacci

package com.taller.seccion2;

import java.util.Scanner;

public class Ejercicio10 {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        System.out.print("Ingrese un número para calcular su Fibonacci: ");
        int n = scanner.nextInt();
        
        System.out.println("El número Fibonacci de " + n + " es: " + fibonacci(n));
        
        scanner.close();
    }
    
    /**
     * Calcula el número Fibonacci de n usando recursión
     * @param n posición en la secuencia Fibonacci
     * @return valor Fibonacci en la posición n
     */
    public static int fibonacci(int n) {
        // Casos base
        if (n <= 0) {
            return 0;
        } else if (n == 1) {
            return 1;
        }
        
        // Caso recursivo
        return fibonacci(n - 1) + fibonacci(n - 2);
    }
}

Ejercicio 11: Leer una lista de números en ArrayList y filtrar pares

package com.taller.seccion2;

import java.util.ArrayList;
import java.util.Scanner;

public class Ejercicio11 {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        ArrayList<Integer> numeros = new ArrayList<>();
        
        System.out.println("Ingrese números (0 para terminar):");
        
        int numero;
        do {
            numero = scanner.nextInt();
            if (numero != 0) {
                numeros.add(numero);
            }
        } while (numero != 0);
        
        System.out.println("Números ingresados: " + numeros);
        
        // Filtrar números pares
        ArrayList<Integer> pares = new ArrayList<>();
        for (Integer num : numeros) {
            if (num % 2 == 0) {
                pares.add(num);
            }
        }
        
        System.out.println("Números pares: " + pares);
        
        scanner.close();
    }
}

Ejercicio 12: Ordenar la lista con Collections.sort

package com.taller.seccion2;

import java.util.ArrayList;
import java.util.Collections;
import java.util.Scanner;

public class Ejercicio12 {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        ArrayList<Integer> numeros = new ArrayList<>();
        
        System.out.println("Ingrese números (0 para terminar):");
        
        int numero;
        do {
            numero = scanner.nextInt();
            if (numero != 0) {
                numeros.add(numero);
            }
        } while (numero != 0);
        
        System.out.println("Lista original: " + numeros);
        
        // Ordenar la lista
        Collections.sort(numeros);
        
        System.out.println("Lista ordenada: " + numeros);
        
        scanner.close();
    }
}

Ejercicio 13: Eliminar duplicados usando un Set

package com.taller.seccion2;

import java.util.ArrayList;
import java.util.HashSet;
import java.util.Scanner;
import java.util.Set;

public class Ejercicio13 {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        ArrayList<Integer> numeros = new ArrayList<>();
        
        System.out.println("Ingrese números (0 para terminar):");
        
        int numero;
        do {
            numero = scanner.nextInt();
            if (numero != 0) {
                numeros.add(numero);
            }
        } while (numero != 0);
        
        System.out.println("Lista con posibles duplicados: " + numeros);
        
        // Eliminar duplicados usando un Set
        Set<Integer> sinDuplicados = new HashSet<>(numeros);
        
        // Convertir de nuevo a ArrayList para mostrar
        ArrayList<Integer> listaSinDuplicados = new ArrayList<>(sinDuplicados);
        
        System.out.println("Lista sin duplicados: " + listaSinDuplicados);
        
        scanner.close();
    }
}

Ejercicio 14: Convertir array a lista con Arrays.asList

package com.taller.seccion2;

import java.util.Arrays;
import java.util.List;

public class Ejercicio14 {
    public static void main(String[] args) {
        // Array original
        String[] colores = {"Rojo", "Verde", "Azul", "Amarillo", "Morado"};
        
        System.out.println("Array original:");
        for (String color : colores) {
            System.out.println("- " + color);
        }
        
        // Convertir array a List usando Arrays.asList
        List<String> listaColores = Arrays.asList(colores);
        
        System.out.println("\nLista convertida:");
        for (String color : listaColores) {
            System.out.println("- " + color);
        }
        
        // Nota: La lista obtenida está respaldada por el array original,
        // cualquier cambio en la lista afectará al array y viceversa
        listaColores.set(0, "Naranja");
        
        System.out.println("\nDespués de modificar la lista, el array queda:");
        for (String color : colores) {
            System.out.println("- " + color);
        }
        
        // Nota: No se pueden agregar o eliminar elementos de la lista resultante
        // listaColores.add("Negro"); // Esto lanzaría UnsupportedOperationException
    }
} 

Sección 3: Arrays y Colecciones (com.taller.seccion3

package com.taller.seccion3;

import java.util.*;

public class Colecciones {
    public static void main(String[] args) {
        // 1. Declara y dimensiona un array de int de tamaño 5
        int[] numeros = new int[5];

        // 2. Inicializa un array literal de String
        String[] nombres = {"Ana", "Luis", "Pedro", "Lucía", "Juan"};

        // 3. Recorre array con índice
        System.out.println("Recorrido con índice:");
        for (int i = 0; i < nombres.length; i++) {
            System.out.println("Índice " + i + ": " + nombres[i]);
        }

        // 4. Recorre array con for-each
        System.out.println("\nRecorrido con for-each:");
        for (String nombre : nombres) {
            System.out.println(nombre);
        }

        // 5. Crea ArrayList<Integer>, añade, elimina y recorre
        ArrayList<Integer> listaEnteros = new ArrayList<>();
        listaEnteros.add(10);
        listaEnteros.add(20);
        listaEnteros.add(30);
        listaEnteros.remove(Integer.valueOf(20)); // Elimina por valor
        System.out.println("\nArrayList:");
        for (int num : listaEnteros) {
            System.out.println(num);
        }

        // 6. Convierte array a ArrayList y viceversa
        List<String> listaNombres = Arrays.asList(nombres);
        String[] nuevoArray = listaNombres.toArray(new String[0]);

        // 7. Usa LinkedList<String> y compara con ArrayList
        LinkedList<String> linkedList = new LinkedList<>();
        linkedList.add("Inicio");
        linkedList.add("Centro");
        linkedList.add("Fin");
        System.out.println("\nLinkedList:");
        for (String s : linkedList) {
            System.out.println(s);
        }

        // 8. Crea HashSet<Double>, añade y muestra tamaño
        HashSet<Double> conjuntoDecimales = new HashSet<>();
        conjuntoDecimales.add(2.5);
        conjuntoDecimales.add(3.14);
        conjuntoDecimales.add(2.5); // Duplicado, no se agrega
        System.out.println("\nTamaño del HashSet: " + conjuntoDecimales.size());

        // 9. Crea HashMap<String, Integer>, mapea nombres a edades
        HashMap<String, Integer> edades = new HashMap<>();
        edades.put("Ana", 25);
        edades.put("Luis", 30);
        edades.put("Pedro", 20);

        // 10. Itera Map.Entry de un HashMap
        System.out.println("\nEntradas del HashMap:");
        for (Map.Entry<String, Integer> entry : edades.entrySet()) {
            System.out.println(entry.getKey() + ": " + entry.getValue());
        }

        // 11. Ordena mapa por valores usando lista auxiliar
        List<Map.Entry<String, Integer>> listaOrdenada = new ArrayList<>(edades.entrySet());
        listaOrdenada.sort(Map.Entry.comparingByValue());
        System.out.println("\nHashMap ordenado por valor:");
        for (Map.Entry<String, Integer> entry : listaOrdenada) {
            System.out.println(entry.getKey() + ": " + entry.getValue());
        }

        // 12. Usa Iterator para eliminar elementos durante iteración
Iterator<Integer> it = listaEnteros.iterator();
        while (it.hasNext()) {
            if (it.next() == 10) {
                it.remove();
            }
        }
        System.out.println("\nArrayList después de eliminar con Iterator:");
        System.out.println(listaEnteros);

        // 13. Chequea contención con contains
 boolean contienePedro = listaNombres.contains("Pedro");
        System.out.println("\n¿Contiene Pedro? " + contienePedro);

        // 14. Limpia colecciones con clear()
  conjuntoDecimales.clear();
        edades.clear();
        System.out.println("\nTamaño HashSet tras clear(): " + conjuntoDecimales.size());
        System.out.println("Tamaño HashMap tras clear(): " + edades.size());
    }
}

       // 15. Reflexiona en Respuestas.md sobre cuándo usar cada colección.

       ## Diferencias entre List, Set y Map

- **List**: Mantiene el orden de inserción, permite elementos duplicados. Ej: ArrayList, LinkedList.
- **Set**: No permite duplicados, no garantiza orden (a menos que uses LinkedHashSet o TreeSet).
- **Map**: Almacena pares clave-valor, no permite claves duplicadas, pero sí valores duplicados.

## ¿Cuándo usar cada colección?

- Usa **List** cuando necesitas acceder a elementos por índice o mantener orden de inserción.
- Usa **Set** cuando necesitas evitar duplicados y no importa el orden.
- Usa **Map** cuando cada elemento tiene una clave única (como nombre → edad).

    Sección 4: Clases, Objetos e Instancias (com.taller.seccion4)

      // 1. Define clase Persona con atributos private String nombre, int edad.

 public class Persona {
    private String nombre;
    private int edad;
    // ...
}

    // 2. Crea constructor con parámetros y constructor sin parámetros (sobrecarga).

    // Constructor sin parámetros
public Persona() {
    this.nombre = "Desconocido";
    this.edad = 0;
    contadorPersonas++;
}

// Constructor con parámetros
public Persona(String nombre, int edad, Direccion direccion) {
    this.nombre = nombre;
    setEdad(edad); // validación incluida
    this.direccion = direccion;
    contadorPersonas++;
}

    // 3. Genera getters y setters con validación (edad >= 0).

 public int getEdad() {
    return edad;
}

public void setEdad(int edad) {
    if (edad >= 0) {
        this.edad = edad;
    } else {
        System.out.println("Edad inválida.");
    }
}

    // 4. Agrega método public void presentarse() que imprima datos.

 public void presentarse() {
    System.out.println("Hola, soy " + nombre + ", tengo " + edad + " años y vivo en " + direccion);
}

    // 5. Crea MainPersona.java y genera 3 objetos con distintos constructores.

 public class MainPersona {
    public static void main(String[] args) {
        Direccion dir1 = new Direccion("Calle 1", "Ciudad A");
        Direccion dir2 = new Direccion("Calle 2", "Ciudad B");

Persona p1 = new Persona(); // sin parámetros
        p1.setNombre("Carlos");
        p1.setEdad(28);
        p1.setDireccion(dir1);

Persona p2 = new Persona("María", 35, dir2); // con parámetros

Persona p3 = new Persona(); // otro con set()
        p3.setNombre("Carlos");
        p3.setEdad(22);
        p3.setDireccion(new Direccion("Calle 3", "Ciudad C"));
    }
}

    // 6. Usa this para diferenciar variables.
    
public Persona(String nombre, int edad, Direccion direccion) {
    this.nombre = nombre;
    this.direccion = direccion;
    setEdad(edad);
}

    // 7.  Declara un atributo static que cuente instancias creadas.

public class Persona {
    private static int contadorInstancias = 0;
    private String nombre;
    private int edad;

 public Persona() {
        contadorInstancias++;
    }

  public Persona(String nombre, int edad) {
        this.nombre = nombre;
        this.edad = edad;
        contadorInstancias++;
    }

public static int getContadorInstancias() {
        return contadorInstancias;
    }
}

    // 8. Implementa método toString() y usa System.out.println(objeto).

    @Override
public String toString() {
    return "Persona{nombre='" + nombre + "', edad=" + edad + "}";
}

Uso:

Persona p = new Persona("Carlos", 30);
System.out.println(p);

    // 9. Sobrescribe equals() y hashCode() basados en nombre.

    @Override
public boolean equals(Object obj) {
    if (this == obj) return true;
    if (obj == null || getClass() != obj.getClass()) return false;
    Persona persona = (Persona) obj;
    return nombre.equals(persona.nombre);
}

@Override
public int hashCode() {
    return nombre.hashCode();
}

    // 10. Documenta con JavaDoc la clase Persona.

    /**
 * Representa una persona con nombre y edad.
 * @author Tú
 */
public class Persona {
    // código...
}

       // 11. Crea clase Direccion y agrégala como atributo de Persona.

   public class Direccion {
    private String calle;
    private String ciudad;

    // constructor, getters y setters
}

public class Persona {
    private Direccion direccion;

    // en constructor: this.direccion = direccion;
}

    // 12. Sobrecarga método presentarse(String saludo).

 public void presentarse(String saludo) {
    System.out.println(saludo + ", soy " + nombre + " y tengo " + edad + " años.");
}

    // 13. Usa final en un método y explica en Respuestas.md.

 public final void metodoFinal() {
    System.out.println("Este método no puede sobrescribirse.");
}

    // 14. Implementa clonación con Cloneable.

public class Persona implements Cloneable {
    @Override
    public Persona clone() throws CloneNotSupportedException {
        return (Persona) super.clone();
    }
}

    // 15. Reflexión: Diferencias entre == y equals().
     En Respuestas.md:

  == compara referencias (si apuntan al mismo objeto), mientras que equals() compara contenido lógico si está sobreescrito.

  Sección 5: Encapsulamiento y Paquetes

    // 1. Mueve Persona y Direccion a com.taller.seccion5.
  (Mover las clases a ese paquete en el IDE Eclipse).

    // 2. Crea paquete util con clase CalculadoraBasica.

    package com.taller.seccion5.util;

public class CalculadoraBasica {
    public static int sumar(int a, int b) { return a + b; }
    public static int restar(int a, int b) { return a - b; }
    public static int multiplicar(int a, int b) { return a * b; }
    public static double dividir(int a, int b) { return a / (double)b; }
}








     
  
