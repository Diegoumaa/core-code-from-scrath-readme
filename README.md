# core-code-from-scrath-readmes
LENGUAJE COMPILADO 

Es un lenguaje de programación de computadora cuyo código fuente generalmente se compila o traduce al código de máquina para producir un programa ejecutable.

Lenguaje interpretado

Es aquel que el código fuente se ejecuta directamente, instrucción a instrucción. Es decir, el código no pasa por un proceso de compilación, sino que tenemos un programa llamado intérprete que lee la instrucción en tiempo real, y la ejecuta

JAVA ES UN LENGUAJE COMPILADO O INTERPRETADO?

Es un lenguaje JAVA es mayormente interpretado; en realidad, usualmente, JAVA se pasa primero a un bytecode que luego es interpretado. El bytecode sería un intermedio entre la programación en lenguaje Java y el código máquina final.
En el caso de Java, lo usual es pasar los programas al bytecode y, al momento de ejecutarlos, se traducen al código máquina para mejorar la velocidad de ejecución. Este paso lo hace la Máquina virtual Java.

  Starting point: START
  Input: READ, GET, GET FROM(<URL>)
  Output: PRINT
  Math: +, -, *, /
  Assignation: <--
  Initialize: SET, INIT
  Add one: INCREMENT
  End point: END
 
   1. START
  2. Amount <-- GET
  3. BTCprice <-- GET
  4. Total <-- Amount * BTCprice
  5. PRINT Total
  9. END
  
  Your date of birth in the matrix?

en decimales es 2000 y en binario es: 11111010000
  
  
  Create a program to add two numbers given by the user
  
  .data

        result: .asciiz "\nEl resultado de la suma es: "
        numero1: .asciiz "\n Escriba el primer numero: "
        numero2: .asciiz "\n Escriba el segundo numero: "
  .text
        main:
  
              li $v0, 4
              la $a0, numero1
              syscall
              li $v0, 5
              syscall
              move $t0, $v0
              li $v0, 4
              la $a0, numero2
              syscall
              li $v0, 5
              syscall
              move $t1, $v0
              add $t2, $t0, $t1
              li $v0, 4
              la $a0, result
              syscall
              li $v0, 1
              move $a0, $t2
              syscall

  Create a program that display your name
  
   .data
	      NOMBRE: .asciiz "\DIEGO UMANA\n"
  .text
	      main:
              li $v0, 4
              la $a0, NOMBRE
              syscall
  
  En este ejercicio debes usar un control de flujo iterativo para poder imprimir todos los números pares en el rango de números del 0 al 100. Recuerda que no debes imprimir cada número, debes usar una estructura de control de flujo para realizar el ejercicio
  
  for (var i = 0; i <= 100; i+=2) {
  
  console.log(i);
}
  
  
