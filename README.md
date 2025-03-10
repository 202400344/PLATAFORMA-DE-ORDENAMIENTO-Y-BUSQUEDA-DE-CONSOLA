# PLATAFORMA-DE-ORDENAMIENTO-Y-BUSQUEDA-DE-CONSOLA
PLATAFORMA DE ORDENAMIENTO  Y BUSQUEDA DE CONSOLA
import java.util.ArrayList;
import java.util.List;
import java.util.Scanner;

public class ProyectoOrdenamiento {

    public static void mostrarInformacion() {
        // Datos fijos del proyecto
        String universidad = "Universidad Da Vinci de Guatemala";
        String curso = "Estructura de Datos";
        String docente = "Ing. Brandon Chitay";

        // Crear un objeto Scanner para leer la entrada del usuario
        Scanner scanner = new Scanner(System.in);

        // Solicitar el nombre del estudiante
        System.out.print("Sandra Ramírez: ");
        String estudiante = scanner.nextLine();
        // Listas de tareas completadas y pendientes
        List<String> puntosHechos = new ArrayList<>();
        List<String> puntosFaltantes = new ArrayList<>();

        // Se inicia el proyecto con el Punto 1 completado
        puntosHechos.add("1. Información del Desarrollador");

        // Lista de tareas restantes
        puntosFaltantes.add("2. Menú Principal");
        puntosFaltantes.add("3. Carga de Datos desde un CSV");
        puntosFaltantes.add("4. Algoritmo de Ordenamiento - Bubble Sort");
        puntosFaltantes.add("5. Algoritmo de Ordenamiento - Enhanced Bubble Sort");
        puntosFaltantes.add("6. Algoritmo de Ordenamiento - Quick Sort");
        puntosFaltantes.add("7. Algoritmo de Ordenamiento - Selection Sort");
        puntosFaltantes.add("8. Algoritmo de Ordenamiento - Merge Sort");
        puntosFaltantes.add("9. Algoritmo de Búsqueda - Binary Search");
        puntosFaltantes.add("10. Presentación Final en YouTube");

        // Mostrar la información en consola
        System.out.println("\n========================================");
        System.out.println(universidad);
        System.out.println(curso);
        System.out.println(docente + "\n");
        System.out.println("Nombre del estudiante: " + estudiante + "\n");

        // Mostrar tareas completadas
        System.out.println("PUNTOS HECHOS:");
        for (String punto : puntosHechos) {
            System.out.println("✅ " + punto);
        }

        // Mostrar tareas pendientes
        System.out.println("\nPUNTOS FALTANTES:");
        for (String punto : puntosFaltantes) {
            System.out.println("❌ " + punto);
        }

        System.out.println("========================================");

        // Esperar a que el usuario presione Enter antes de continuar
        System.out.println("Presione Enter para continuar...");
        scanner.nextLine();  // Captura la entrada del usuario

        // Cerrar el scanner
        scanner.close();
    }

    public static void main(String[] args) {
        mostrarInformacion();  // Llamamos a la función para ejecutarla
    }
}
import java.util.ArrayList;
import java.util.List;
import java.util.Scanner;

public class ProyectoOrdenamiento {

    public static void mostrarInformacion() {
        // Datos fijos del proyecto
        String universidad = "Universidad Da Vinci de Guatemala";
        String curso = "Estructura de Datos";
        String docente = "Ing. Brandon Chitay";

        // Crear un objeto Scanner para leer la entrada del usuario
        Scanner scanner = new Scanner(System.in);

        // Solicitar el nombre del estudiante
        System.out.print("Ingrese su nombre: ");
        String estudiante = scanner.nextLine();

        // Listas de tareas completadas y pendientes
        List<String> puntosHechos = new ArrayList<>();
        List<String> puntosFaltantes = new ArrayList<>();

        // Se inicia el proyecto con los primeros puntos completados
        puntosHechos.add("1. Información del Desarrollador");
        puntosHechos.add("2. Menú Principal");

        // Lista de tareas restantes
        puntosFaltantes.add("3. Carga de Datos desde un CSV");
        puntosFaltantes.add("4. Algoritmo de Ordenamiento - Bubble Sort");
        puntosFaltantes.add("5. Algoritmo de Ordenamiento - Enhanced Bubble Sort");
        puntosFaltantes.add("6. Algoritmo de Ordenamiento - Quick Sort");
        puntosFaltantes.add("7. Algoritmo de Ordenamiento - Selection Sort");
        puntosFaltantes.add("8. Algoritmo de Ordenamiento - Merge Sort");
        puntosFaltantes.add("9. Algoritmo de Búsqueda - Binary Search");
        puntosFaltantes.add("10. Presentación Final en YouTube");

        // Mostrar la información en consola
        System.out.println("\n========================================");
        System.out.println(universidad);
        System.out.println(curso);
        System.out.println(docente + "\n");
        System.out.println("Nombre del estudiante: " + estudiante + "\n");

        // Mostrar tareas completadas
        System.out.println("PUNTOS HECHOS:");
        for (String punto : puntosHechos) {
            System.out.println("✅ " + punto);
        }

        // Mostrar tareas pendientes
        System.out.println("\nPUNTOS FALTANTES:");
        for (String punto : puntosFaltantes) {
            System.out.println("❌ " + punto);
        }

        System.out.println("========================================");

        // Esperar a que el usuario presione Enter antes de continuar
        System.out.println("Presione Enter para continuar...");
        scanner.nextLine();  // Captura la entrada del usuario

        // Llamar al menú principal
        mostrarMenu(scanner);
    }

    public static void mostrarMenu(Scanner scanner) {
        int opcion;
        do {
            // Mostrar opciones
            System.out.println("\n========== MENÚ PRINCIPAL ==========");
            System.out.println("1. Cargar datos desde un archivo CSV");
            System.out.println("2. Ordenar datos usando Bubble Sort");
            System.out.println("3. Ordenar datos usando Enhanced Bubble Sort");
            System.out.println("4. Ordenar datos usando Quick Sort");
            System.out.println("5. Ordenar datos usando Selection Sort");
            System.out.println("6. Ordenar datos usando Merge Sort");
            System.out.println("7. Buscar un número con Binary Search");
            System.out.println("8. Salir");
            System.out.print("Ingrese una opción: ");

            // Leer opción del usuario
            opcion = scanner.nextInt();
            scanner.nextLine();  // Limpiar el buffer

            // Ejecutar la acción correspondiente
            switch (opcion) {
                case 1:
                    System.out.println("📂 Opción seleccionada: Cargar datos desde un CSV (Pendiente de implementación).");
                    break;
                case 2:
                    System.out.println("🔄 Opción seleccionada: Bubble Sort (Pendiente de implementación).");
                    break;
                case 3:
                    System.out.println("🔄 Opción seleccionada: Enhanced Bubble Sort (Pendiente de implementación).");
                    break;
                case 4:
                    System.out.println("⚡ Opción seleccionada: Quick Sort (Pendiente de implementación).");
                    break;
                case 5:
                    System.out.println("🎯 Opción seleccionada: Selection Sort (Pendiente de implementación).");
                    break;
                case 6:
                    System.out.println("🔀 Opción seleccionada: Merge Sort (Pendiente de implementación).");
                    break;
                case 7:
                    System.out.println("🔎 Opción seleccionada: Binary Search (Pendiente de implementación).");
                    break;
                case 8:
                    System.out.println("👋 Saliendo del programa...");
                    break;
                default:
                    System.out.println("⚠️ Opción no válida. Intente de nuevo.");
            }
        } while (opcion != 8);
    }

    public static void main(String[] args) {
        mostrarInformacion();  // Llamamos a la función principal
    }
}
import java.io.*;
import java.util.*;

public class CargaDatosCSV {
    public static List<Integer> cargarDatos(String nombreArchivo) {
        List<Integer> datos = new ArrayList<>();
        try (BufferedReader br = new BufferedReader(new FileReader(nombreArchivo))) {
            String linea;
            while ((linea = br.readLine()) != null) {
                try {
                    datos.add(Integer.parseInt(linea.trim()));
                } catch (NumberFormatException e) {
                    System.out.println("⚠️ Dato inválido en el archivo: " + linea);
                }
            }
            System.out.println("✅ Datos cargados exitosamente desde " + nombreArchivo);
        } catch (IOException e) {
            System.out.println("❌ Error al leer el archivo: " + e.getMessage());
        }
        return datos;
    }

    public static void opcionCargarDatos(Scanner scanner, List<Integer> listaDatos) {
        System.out.print("📂 Ingrese el nombre del archivo CSV: ");
        String nombreArchivo = scanner.nextLine();
        List<Integer> datosCargados = cargarDatos(nombreArchivo);
        if (!datosCargados.isEmpty()) {
            listaDatos.clear();
            listaDatos.addAll(datosCargados);
        }
    }
}List<Integer> listaDatos = new ArrayList<>();

// En la función mostrarMenu()
case 1:
    CargaDatosCSV.opcionCargarDatos(scanner, listaDatos);
    break;
    import java.util.List;

public class BubbleSort {
    public static void ordenar(List<Integer> lista) {
        int n = lista.size();
        for (int i = 0; i < n - 1; i++) {
            for (int j = 0; j < n - i - 1; j++) {
                if (lista.get(j) > lista.get(j + 1)) {
                    // Intercambiar elementos
                    int temp = lista.get(j);
                    lista.set(j, lista.get(j + 1));
                    lista.set(j + 1, temp);
                }
            }
        }
        System.out.println("✅ Lista ordenada con Bubble Sort.");
    }

    public static void opcionBubbleSort(List<Integer> lista) {
        if (lista.isEmpty()) {
            System.out.println("❌ No hay datos cargados. Cargue datos primero.");
            return;
        }
        ordenar(lista);
        System.out.println("📊 Lista ordenada: " + lista);
    }
}import java.util.List;

public class EnhancedBubbleSort {
    public static void ordenar(List<Integer> lista) {
        int n = lista.size();
        boolean intercambiado;
        
        for (int i = 0; i < n - 1; i++) {
            intercambiado = false;
            
            for (int j = 0; j < n - i - 1; j++) {
                if (lista.get(j) > lista.get(j + 1)) {
                    // Intercambiar elementos
                    int temp = lista.get(j);
                    lista.set(j, lista.get(j + 1));
                    lista.set(j + 1, temp);
                    intercambiado = true;
                }
            }
            
            // Si no hubo intercambios, la lista ya está ordenada
            if (!intercambiado) break;
        }
        System.out.println("✅ Lista ordenada con Enhanced Bubble Sort.");
    }

    public static void opcionEnhancedBubbleSort(List<Integer> lista) {
        if (lista.isEmpty()) {
            System.out.println("❌ No hay datos cargados. Cargue datos primero.");
            return;
        }
        ordenar(lista);
        System.out.println("📊 Lista ordenada: " + lista);
    }
}import java.util.List;

public class QuickSort {
    public static void ordenar(List<Integer> lista, int inicio, int fin) {
        if (inicio < fin) {
            int indicePivote = particion(lista, inicio, fin);
            ordenar(lista, inicio, indicePivote - 1);
            ordenar(lista, indicePivote + 1, fin);
        }
    }

    private static int particion(List<Integer> lista, int inicio, int fin) {
        int pivote = lista.get(fin);  // Elegimos el último elemento como pivote
        int i = inicio - 1;

        for (int j = inicio; j < fin; j++) {
            if (lista.get(j) < pivote) {
                i++;
                // Intercambiar lista[i] y lista[j]
                int temp = lista.get(i);
                lista.set(i, lista.get(j));
                lista.set(j, temp);
            }
        }

        // Intercambiar el pivote con lista[i+1] para colocarlo en su posición final
        int temp = lista.get(i + 1);
        lista.set(i + 1, lista.get(fin));
        lista.set(fin, temp);

        return i + 1;  // Retornamos la posición del pivote
    }

    public static void opcionQuickSort(List<Integer> lista) {
        if (lista.isEmpty()) {
            System.out.println("❌ No hay datos cargados. Cargue datos primero.");
            return;
        }
        ordenar(lista, 0, lista.size() - 1);
        System.out.println("✅ Lista ordenada con Quick Sort.");
        System.out.println("📊 Lista ordenada: " + lista);
    }
}import java.util.List;

public class SelectionSort {
    public static void ordenar(List<Integer> lista) {
        int n = lista.size();
        for (int i = 0; i < n - 1; i++) {
            int indiceMinimo = i;
            for (int j = i + 1; j < n; j++) {
                if (lista.get(j) < lista.get(indiceMinimo)) {
                    indiceMinimo = j;
                }
            }
            // Intercambiar el mínimo encontrado con el primer elemento no ordenado
            int temp = lista.get(i);
            lista.set(i, lista.get(indiceMinimo));
            lista.set(indiceMinimo, temp);
        }
        System.out.println("✅ Lista ordenada con Selection Sort.");
    }

    public static void opcionSelectionSort(List<Integer> lista) {
        if (lista.isEmpty()) {
            System.out.println("❌ No hay datos cargados. Cargue datos primero.");
            return;
        }
        ordenar(lista);
        System.out.println("📊 Lista ordenada: " + lista);
    }import java.util.List;
import java.util.ArrayList;

public class MergeSort {
    public static void ordenar(List<Integer> lista) {
        if (lista.size() < 2) {
            return; // Caso base: lista con un solo elemento ya está ordenada
        }

        int mitad = lista.size() / 2;
        List<Integer> izquierda = new ArrayList<>(lista.subList(0, mitad));
        List<Integer> derecha = new ArrayList<>(lista.subList(mitad, lista.size()));

        ordenar(izquierda);
        ordenar(derecha);
        
        merge(lista, izquierda, derecha);
    }

    private static void merge(List<Integer> lista, List<Integer> izquierda, List<Integer> derecha) {
        int i = 0, j = 0, k = 0;

        // Mezclar las dos listas ordenadas
        while (i < izquierda.size() && j < derecha.size()) {
            if (izquierda.get(i) < derecha.get(j)) {
                lista.set(k++, izquierda.get(i++));
            } else {
                lista.set(k++, derecha.get(j++));
            }
        }

        // Si quedan elementos en la lista izquierda
        while (i < izquierda.size()) {
            lista.set(k++, izquierda.get(i++));
        }

        // Si quedan elementos en la lista derecha
        while (j < derecha.size()) {
            lista.set(k++, derecha.get(j++));
        }
    }

    public static void opcionMergeSort(List<Integer> lista) {
        if (lista.isEmpty()) {
            System.out.println("❌ No hay datos cargados. Cargue datos primero.");
            return;
        }
        ordenar(lista);
        System.out.println("✅ Lista ordenada con Merge Sort.");
        System.out.println("📊 Lista ordenada: " + lista);
    }
}public class BinarySearch {
    public static int buscar(List<Integer> lista, int objetivo) {
        int inicio = 0;
        int fin = lista.size() - 1;

        while (inicio <= fin) {
            int medio = inicio + (fin - inicio) / 2;
            
            // Si encontramos el elemento
            if (lista.get(medio) == objetivo) {
                return medio; // Devuelve el índice del elemento
            }
            
            // Si el objetivo es mayor que el elemento medio
            if (lista.get(medio) < objetivo) {
                inicio = medio + 1;
            } 
            // Si el objetivo es menor que el elemento medio
            else {
                fin = medio - 1;
            }
        }
        
        return -1; // Si el elemento no está presente en la lista
    }

    public static void opcionBinarySearch(List<Integer> lista) {
        if (lista.isEmpty()) {
            System.out.println("❌ No hay datos cargados. Cargue datos primero.");
            return;
        }
        
        System.out.print("Ingrese el número que desea buscar: ");
        int objetivo = new java.util.Scanner(System.in).nextInt();
        
        int resultado = buscar(lista, objetivo);
        
        if (resultado == -1) {
            System.out.println("❌ El número no está en la lista.");
        } else {
            System.out.println("✅ El número " + objetivo + " se encuentra en el índice: " + resultado);
        }
    }
}import java.io.BufferedReader;
import java.io.FileReader;
import java.io.IOException;
import java.util.List;
import java.util.ArrayList;

public class CargarDatosCSV {

    public static List<Integer> cargarDesdeCSV(String archivo) {
        List<Integer> lista = new ArrayList<>();
        
        try (BufferedReader br = new BufferedReader(new FileReader(archivo))) {
            String linea;
            while ((linea = br.readLine()) != null) {
                String[] numeros = linea.split(",");
                for (String num : numeros) {
                    try {
                        lista.add(Integer.parseInt(num.trim())); // Convertir y agregar a la lista
                    } catch (NumberFormatException e) {
                        System.out.println("❌ Error al procesar el número: " + num);
                    }
                }
            }
        } catch (IOException e) {
            System.out.println("❌ Error al leer el archivo: " + e.getMessage());
        }
        
        return lista;
    }

    public static void opcionCargarDatos(List<Integer> lista) {
        System.out.print("Ingrese la ruta del archivo CSV: ");
        String archivo = new java.util.Scanner(System.in).nextLine();
        
        lista.clear();  // Limpiar la lista antes de cargar nuevos datos
        List<Integer> datosCargados = cargarDesdeCSV(archivo);
        
        if (datosCargados.isEmpty()) {
            System.out.println("❌ No se cargaron datos del archivo.");
        } else {
            lista.addAll(datosCargados);
            System.out.println("✅ Datos cargados correctamente.");
            System.out.println("📊 Datos cargados: " + lista);
        }
    }
}


