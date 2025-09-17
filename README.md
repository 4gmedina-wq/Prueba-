\# 🧩 Prueba Técnica Semisenior — Solución en C#



Autor: \*\*Guillermo Alberto Medina Garcés\*\*  

Cargo: \*\*Analista Programador Semisenior\*\*  

Fecha: \*\*Septiembre 2025\*\*



---



\## 📌 Descripción del Problema



Un grupo de excursionistas necesita elegir un conjunto de alimentos que cumpla con estas condiciones:



1\. Alcanzar un \*\*mínimo de calorías requeridas\*\*.  

2\. No superar un \*\*peso máximo permitido\*\*.  

3\. Minimizar el \*\*peso total\*\* de los ítems seleccionados.  



En otras palabras, es una variación del clásico \*\*Problema de la Mochila (Knapsack Problem)\*\*, optimizado para minimizar el peso sujeto a un umbral de calorías.



\*\*Ejemplo (del enunciado):\*\*



\- Calorías mínimas: 15  

\- Peso máximo: 10  

\- Elementos:  

&nbsp; - E1 → 5kg, 3cal  

&nbsp; - E2 → 3kg, 5cal  

&nbsp; - E3 → 5kg, 2cal  

&nbsp; - E4 → 1kg, 8cal  

&nbsp; - E5 → 2kg, 3cal  



✅ Mejor combinación: \*\*E2 + E4\*\* (peso = 4kg, calorías = 13).  

⚠️ Nota: Si se requieren exactamente 15 calorías, pueden añadirse otros ítems según el caso.



---



\## 💡 Solución Propuesta



La primera versión del algoritmo fue un \*\*backtracking recursivo\*\*, correcto pero ineficiente para muchos elementos (`O(2^n)`).  

La versión final implementa \*\*Programación Dinámica (DP)\*\* para optimizar tiempo y memoria (`O(n × calorías)`).



\### ✅ Ventajas de esta solución:

\- Escalable a decenas o cientos de ítems.  

\- Siempre encuentra la combinación óptima con \*\*peso mínimo\*\*.  

\- Reconstrucción de la solución paso a paso.  

\- Interfaz de consola amigable para ingresar datos manualmente.  



---



\## 🖥️ Ejecución del Programa



\### 1. Requisitos

\- \[.NET SDK 6.0+](https://dotnet.microsoft.com/en-us/download)  



\### 2. Compilación y Ejecución

```bash

\# Compilar

csc Program.cs



\# Ejecutar

Program.exe



