# **Universidad Nacional de Colombia**
## **Programación de Computadores (Código 2015734)**
### **Repositorio elaborado por**: Santiago Romero Mejía

>**Objetivo**: Plantear un algoritmo que obtenga los números primos hasta un número n, empleando pseudocódigo y diagramas de flujo.

**Desarrollo**: Creamos una lista con todos los números naturales hasta un número n. Cualquier número k de la lista es primo si es divisible únicamente por 1 y por sí mismo, en otras palabras, si dividimos k entre cada uno de los números naturales menores a él (incluyéndolo), debemos obtener que el residuo de la división es 0 únicamente cuando los divisores son 1 y k.
Para efectos prácticos, si planteamos esta misma división sin incluir como divisores a 1 y k, entonces debemos obtener que k es primo si para todo i < k se cumple: k / i != 0.

El planteamiento en pseudocódigo se desarrolla de la siguiente forma:
```pseudocode
[Variables]
n : entero
k : entero
i : entero
inicio
    k := 2
    i := 2
    Mientras (k < n + 1) hacer
        Si modulo (k, i) == 0 entonces
            escribir ("k es compuesto")
        sino
            Si (i > k/2) entonces  
                escribir ("k es primo")
                k := k + 1
                i := 2
            sino
                i := i + 1
    Fin mientras
fin
```
El algoritmo estructurado en un diagrama de flujo se desarrolla de la siguiente forma:
[![](https://mermaid.ink/img/pako:eNpNkc1ugkAQx19lsidNNbb2RipJFdESsQc9AR42sMoG2SXrkqYBH6Ev1Ksv1llAy55mf_Of74rEMmHEIsez_IpTqjTsnUgAvvfBh-Axl0MYj-15KG6_OVMSBNjwemglc-NahFNgFygUz2XHF4Y7YQYzmHbIMWgZ8h5aGuSiagIGqw67BsOqUsiery1bGVbvbj_1GvVYLZZ5UbKLlgfj7ou2n7VXcbBnkE2mXbh392ybBjg8wUtXzbsn3rSJ-2NsTJjfjJH1QtYNbu1tM0Nr-8YOqgzecEko74oHj96XfYDd7AYuF0MyIrjYnPIEz1AZSUR0ynIWEQvNhKosIpG4oo6WWu6-RUwsrUo2IkqWp5RYR3q-4K8sEqqZw-lJ0fxBCyoCKf__LOFaKr-9enP86x8zjZWi?type=png)](https://mermaid.live/edit#pako:eNpNkc1ugkAQx19lsidNNbb2RipJFdESsQc9AR42sMoG2SXrkqYBH6Ev1Ksv1llAy55mf_Of74rEMmHEIsez_IpTqjTsnUgAvvfBh-Axl0MYj-15KG6_OVMSBNjwemglc-NahFNgFygUz2XHF4Y7YQYzmHbIMWgZ8h5aGuSiagIGqw67BsOqUsiery1bGVbvbj_1GvVYLZZ5UbKLlgfj7ou2n7VXcbBnkE2mXbh392ybBjg8wUtXzbsn3rSJ-2NsTJjfjJH1QtYNbu1tM0Nr-8YOqgzecEko74oHj96XfYDd7AYuF0MyIrjYnPIEz1AZSUR0ynIWEQvNhKosIpG4oo6WWu6-RUwsrUo2IkqWp5RYR3q-4K8sEqqZw-lJ0fxBCyoCKf__LOFaKr-9enP86x8zjZWi)

**Resultados**: El problema planteado es solucionable algorítmicamente.
