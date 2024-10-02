# practica-6-Java-Two-Pointers-Technique

La tecnica de Two Pointers es util para

Existen 3 variantes: Misma direccion, direccion opuesta y sliding window.

Resuelve los siguientes problemas usando Two Pointers.

Direccion opuesta.

Dado un array ordenado de enteros, encuentra si existen dos números en el array cuya suma sea igual a un número objetivo. Usa dos punteros donde uno comienza desde el inicio y el otro desde el final.

```Java
class TwoSumOppositePointers {
    /* Escribe tu codigo aqui */

    public static void runTests() {
        int[] nums1 = {1, 2, 3, 4, 5};
        int target1 = 9;
        System.out.println("Tu respuesta es: " + hasPairWithSum(nums1, target1));
        System.out.println("La salida es: " + (hasPairWithSum(nums1, target1) ? "Test Passed" : "Test Failed"));

        int[] nums2 = {1, 2, 3, 7, 10};
        int target2 = 6;
        System.out.println("Tu respuesta es: " + hasPairWithSum(nums2, target2));
        System.out.println("La salida es: " + (hasPairWithSum(nums2, target2) ? "Test Passed" : "Test Failed"));

        int[] nums3 = {-1, 0, 1, 2};
        int target3 = 0;
        System.out.println("Tu respuesta es: " + hasPairWithSum(nums3, target3));
        System.out.println("La salida es: " + (hasPairWithSum(nums3, target3) ? "Test Passed" : "Test Failed"));
    }

    public static void main(String[] args) {
        runTests();
    }
}

```

Misma direccion
Dado un array de enteros, encuentra si hay dos números en el array cuya suma sea igual a un número objetivo. Usa dos punteros donde ambos comienzan desde la misma posición y se mueven para encontrar la suma deseada.

```Java
class TwoSumEqualPointers {
    /* Escribe tu codigo aqui */

    public static void runTests() {
        int[] nums1 = {1, 2, 3, 4, 5};
        int target1 = 9;
        System.out.println("Tu respuesta es: " + hasPairWithSum(nums1, target1));
        System.out.println("La salida es: " + (hasPairWithSum(nums1, target1) ? "Test Passed" : "Test Failed"));

        int[] nums2 = {1, 2, 3};
        int target2 = 6;
        System.out.println("Tu respuesta es: " + hasPairWithSum(nums2, target2));
        System.out.println("La salida es: " + (hasPairWithSum(nums2, target2) ? "Test Passed" : "Test Failed"));

        int[] nums3 = {-1, 0, 1, 2};
        int target3 = 0;
        System.out.println("Tu respuesta es: " + hasPairWithSum(nums3, target3));
        System.out.println("La salida es: " + (hasPairWithSum(nums3, target3) ? "Test Passed" : "Test Failed"));
    }

    public static void main(String[] args) {
        runTests();
    }
}

```
Salida: 
```
Tu respuesta es: true
La salida es: Test Passed
Tu respuesta es: false
La salida es: Test Passed
Tu respuesta es: true
La salida es: Test Passed
```

Sliding window

Dado un array de enteros, encuentra el subarray de tamaño k que tiene la suma máxima. Usa una ventana deslizante para calcular la suma del subarray en cada iteración.

```Java
class MaxSumSlidingWindow {
    /* Escribe tu codigo aqui */

    public static void runTests() {
        int[] nums1 = {1, 2, 3, 4, 5};
        int k1 = 2;
        System.out.println("Tu respuesta es: " + maxSumSubarray(nums1, k1));
        System.out.println("La salida es: " + (maxSumSubarray(nums1, k1) == 9 ? "Test Passed" : "Test Failed"));

        int[] nums2 = {1, -1, 3, -2, 5};
        int k2 = 3;
        System.out.println("Tu respuesta es: " + maxSumSubarray(nums2, k2));
        System.out.println("La salida es: " + (maxSumSubarray(nums2, k2) == 6 ? "Test Passed" : "Test Failed"));

        int[] nums3 = {10, 2, -10, 5, 3};
        int k3 = 2;
        System.out.println("Tu respuesta es: " + maxSumSubarray(nums3, k3));
        System.out.println("La salida es: " + (maxSumSubarray(nums3, k3) == 12 ? "Test Passed" : "Test Failed"));
    }

    public static void main(String[] args) {
        runTests();
    }
}
```
Salida esperada: 
```
Tu respuesta es: 9
La salida es: Test Passed
Tu respuesta es: 6
La salida es: Test Passed
Tu respuesta es: 12
La salida es: Test Passed
```
