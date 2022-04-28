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
	
	function multiply(a, b){ return a * b;}
	
	ASCII Total
	
function uniTotal(string) {return Array.from(string).reduce( (result, char) => result + char.charCodeAt(0),0);}
	
	Char From ASCII Value

	function  getChar(c) {return String.fromCharCode(c);}
	
	Binary Addition

	function addBinary(a, b) {return (a + b).toString(2);}
	
	Student's Final Grade
	
function finalGrade(exam, projects) {let resultado = 0; if (exam > 90 || projects > 10) resultado = 100;} else if (exam > 75 && projects >= 5) {resultado = 90;} else if (exam > 50 && projects >= 2) {
    resultado = 75;
  }
  return resultado;
}
	
	Holiday VIII - Duty Free

	function dutyFree(normPrice, discount, hol) {let dicountPrice = (normPrice * discount) / 100;
   let bottlesWithDicountPriceToCoverHoliday = hol / dicountPrice;
  let roundedResult = Math.floor(bottlesWithDicountPriceToCoverHoliday);
  return roundedResult;}
	
	Twice As Old
	
function twiceAsOld(dadYearsOld, sonYearsOld) { return Math.abs(dadYearsOld - 2 * sonYearsOld);}
	
	Valid Spacing
	
	function validSpacing(s) {
  if (s.length === 0) return true;
  if (s[0] === ' ' || s[s.length - 1] === ' ') return false;
  let aSpaces0 = s.split(' ');
  for (let i = 0, length = aSpaces0.length; i < length; i++) {
    if (aSpaces0[i] === '') return false;
  }
  return true;
}
	
						       Fake Binary

						       function fakeBin(x) {
  return Array.from(x)
    .map((digit) => (+digit < 5 ? 0 : 1))
    .join('');
}
			       Remove All Exclamation Marks From The End Of Sentence
function remove(string) {
  return string.replace(/!+$/, '');
}
			       Vowel Remover

			       function shortcut(string) {
  return string.replace(/[aeiou]/g, '');
}
			       Rock Paper Scissors!
const rps = (p1, p2) => {
  let rules = { rock: 'scissors', paper: 'rock', scissors: 'paper' };
  if (p1 === p2) return 'Draw!';
  if (p2 === rules[p1]) {
    return 'Player 1 won!';
  }
  return 'Player 2 won!';
};
	Persistent Bugger

	
function persistence(num) {
  let times = 0;
  num = num.toString();
  while (num.length > 1) {
    times++;
    num = num
      .split('')
      .map((a) => Number(a))
      .reduce((a, b) => a * b)
      .toString();
  }
  return times;
}
	week 3
	
	Who Likes It?
	
	function likes(names) {
  if (names.length == 0) return 'no one likes this';
  if (names.length == 1) return `${names[0]} likes this`;
  if (names.length == 2) return `${names[0]} and ${names[1]} like this`;
  if (names.length == 3)
    return `${names[0]}, ${names[1]} and ${names[2]} like this`;
  return `${names[0]}, ${names[1]} and ${names.length - 2} others like this`;
}
	
	Bit Counting
	
var countBits = function (n) {
  return n
    .toString(2)
    .split('')
    .reduce((total, val) => total + Number(val), 0);
};
	
	Your order, please
	
function order(words) {
  let wordsArray = words.split(' ');
  wordsArray = wordsArray.sort(
    (w1, w2) => Number(w1.replace(/\D/g, '')) - Number(w2.replace(/\D/g, ''))
  );
  return wordsArray.join(' ');
}

	Simple Pig Latin

	function pigIt(str) {
  return str.replace(/(\w)(\w*)(\s|$)/g, '$2$1ay$3');
}
	
Counting Duplicates

	function duplicateCount(text) {
  return text
    .toLowerCase()
    .split('')
    .filter((char, i, arr) => {
      return arr.indexOf(char) !== i && arr.lastIndexOf(char) === i;
    }).length;
}
	
	Decode The Morse Code

	decodeMorse = function (morseCode) {
  return morseCode
    .split(' ')
    .map((word) => MORSE_CODE[word] || ' ')
    .join('')
    .replace(/  /g, ' ')
    .trim();
};
	
	Valid Parentheses

	
	function validParentheses(parens) {
  return [...parens].reduce((a, c) => (a + c).replace('()', ''), '') === '';
}
	
Convert String To Camel Case

	function toCamelCase(str) {
  return str
    .replace(/-/g, '_')
    .split('_')
    .map((word, i) => (i > 0 ? word.toUpperCase()[0] + word.substr(1) : word))
    .join('');
};
	
	
	Unique In Order
	
var uniqueInOrder = function (iterable) {
  return [...iterable].filter((chr, i) => chr != iterable[i + 1]);
};
	
	
