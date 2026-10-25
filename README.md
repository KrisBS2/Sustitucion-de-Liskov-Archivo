Principio Sustitución de Liskov (LSP)
El principio se implementa en este con:

1. **Uso de métodos virtuales y sobrescritura (`override`):** La clase base `Producto` define un método virtual `AplicarDescuento()`, el cual es sobrescrito adecuadamente en las clases derivadas `Fisico` y `Digital`
2. **Sustitución correcta sin alterar el comportamiento:** Las clases hijas pueden reemplazar a la clase base en cualquier momento, permitiendo que el método general `ConvertirPrecio()` ejecute el cálculo de descuento específico de cada tipo (`30%` para físico y `12%` para digital) de forma transparente y sin romper la lógica del programa
