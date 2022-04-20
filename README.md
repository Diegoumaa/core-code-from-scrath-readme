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
  
The code shown below is not working in the right way, as a task you must find the error made by the developer who programmed this code and correct it, for this exercise you must explain what the error is and place the correct code
			  
	FORMA INCORRECTA
			  
var cond = false;

if ((cond = true)) {
			  
  console.log('The cond variable is true');
			  
}
			  else 
			  {
  console.log('The cond variable is false');
			  
}
			  
	FORMA CORRECTA	
			  
var  cond  =  false ;

if (cond) {
			  
  console.log('es verdadero');
			  
} 
			  else {
			  
  console.log('es falso');
			  
}
			  
EL ERROR CON EL PRIMER CODIGO ES QUE A LA VARIABLE "COND" TENIA EL VALOR DE FALSE ENTONCES CUANDO ENTRA AL IF TENIA QUE SER VALOR TRUE ENTONCES NO CONCUERDA CON LA SENTENCIA EN CAMBIO SI DEJAMOS QUE TODO FLUYA NORMALMENTE COMO EL CODIGO CORECTO TENEMOS LA RESPUESTA QUE DEBERIA SER.
			  
 Debes crear el código que sigue la siguiente lógica, si el número dado es 100, toma este número como especial y muestra el siguiente mensaje: "¡Este es un número especial!", pero si el número es menor que 1000, múltiplo de 10 y diferente de 100, debe mostrar el siguiente mensaje: "Este número es casi especial". si no se cumple ninguna de las condiciones dadas mostrar el siguiente mensaje: "Sólo un número regular". Otro desarrollador estaba tratando de programar la lógica, pero aparentemente no pudo, necesita corregir el código para que funcione correctamente.
			  
			  
 var  valor  =  100 ;

if (valor == 100) {
  console.log('este numero es especial!');
} else if (valor < 1000 && valor % 10 == 0) {
  console.log('este numero es casi especial');
} else {
  console.log('numero regular');
}
	
	
	MULTIPLICAR
	function multiply(a, b){
 return a * b;
}
	ASCII Total
function uniTotal(string) {
  return Array.from(string).reduce(
    (result, char) => result + char.charCodeAt(0),0);
}
	Binary Addition
function addBinary(a, b) {
  return (a + b).toString(2);
}
	Student's Final Grade
function finalGrade(exam, projects) {
  let resultado = 0;
  if (exam > 90 || projects > 10) {
    resultado = 100;
  } else if (exam > 75 && projects >= 5) {
    resultado = 90;
  } else if (exam > 50 && projects >= 2) {
    resultado = 75;
  }
  return resultado;
}
