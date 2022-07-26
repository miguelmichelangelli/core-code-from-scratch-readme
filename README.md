<h1 align="center">My Readme</h>

<h2>Index</h2>
        
1. [Week 1](#week-1)
2. [Week 2](#week-2)
3. [Week 3](#week-3)
4. [Week 4](#week-4)
5. [Week 5](#week-5)
6. [Week 6](#week-6)

<h2 id="week-1">Week 1</h2>
    <h3>Tuesday</h3>
        <p><b>Assignation 1: Create an explanation about Interpreted And Compiled Programming Languages</b></p<>
        <p>Compiled language:<br>
        This type of language translate the source code into machine code directly by the target machine, they use to be faster than interpreted languages for this reason. Examples of Compiled Languages are C, C++, Erlang, Haskell, Rust, and Go. </p>
        <br>
        <p>Interpreted Languages:<br>
        Instead, in the Interpreted Language a program (also know as interpreter) is who reads and executes the code, not the target machine directly. This type of language is a little slower than the compiled one, but also is more flexible and the program size is smaller. Examples of Interpreted Languages are PHP, Ruby, Python, and JavaScript. </p>
<br>
        <p><b>Assignation 2: Is Java compiled or interpreted, or both?</b></p>
        <p>Java can be considered as both of this languages, because its source code is first compiled into a binary byte-code by the Java compiler, then this byte-code is executed by the Java Virtual Machine (JVM) which is usually a software-based interpreter. </p>
<br>
        <p><b>Assignation 3: Pseudo currency converter excersice</b></p>
        <p>
        Task List:
                <ul>
                        <li>Starting point: START</li>
                        <li>Input: GET, GET FROM("URL")</li>
                        <li>Output: PRINT
                        <li>Math: +, -, *, /</li>
                        <li>Assignation: <-- </li>
                        <li>End point: END</li>
                </ul>
        Algorithm:
                <ol>
                        <li>START</li>
                        <li>Amount <-- GET</li>
                        <li>Bitcoin-price <-- GET FROM(https://www.coindesk.com/price/bitcoin/)</li>
                        <li>T <-- Amount * Bitcoin-price</li>
                        <li>PRINT T</li>
                        <li>END</li>
                </ol>
        </p>
<br>
        <p><b>Assignation 4:</b> Learn about high and low level languages</p>
                <p>The High Level Languages are user-orientated, have been made for programmers to convert an algorithm into program code easily. These require the use of a compiler or interpreter for the translation of the algorithm into machin code, some examples are JavaScript, Python, HTML, C++...

<br>
                The Low Level Languages instead are machine-orientated, can be executed in the computer hardware without any compiler or interpreter. Some examples are asembly language or machin code.</p>
<br>

   <h3>Wednesday</h3>
        <p><b>Assignation 1:</b> Your date of birth in the Matrix?</p>
                <p>Date of birth: 2003</p>
                <table border="2px">
                        <tr>
                           <td>2<sup>10</sup></td>
                           <td>2<sup>9</sup></td>
                           <td>2<sup>8</sup></td>
                           <td>2<sup>7</sup></td>
                           <td>2<sup>6</sup></td>
                           <td>2<sup>5</sup></td>
                           <td>2<sup>4</sup></td>
                           <td>2<sup>3</sup></td>
                           <td>2<sup>2</sup></td>
                           <td>2<sup>1</sup></td>
                           <td>2<sup>0</sup></td>
                        </tr>
                        <tr>
                           <td>1024</td>
                           <td>512</td>
                           <td>256</td>
                           <td>128</td>
                           <td>64</td>
                           <td>32</td>
                           <td>16</td>
                           <td>8</td>
                           <td>4</td>
                           <td>2</td>
                           <td>1</td>
                        </tr>
                           <td><b>1</b></td>
                           <td><b>1</b></td>
                           <td><b>1</b></td>
                           <td><b>1</b></td>
                           <td><b>1</b></td>
                           <td><b>0</b></td>
                           <td><b>1</b></td>
                           <td><b>0</b></td>
                           <td><b>0</b></td>
                           <td><b>1</b></td>
                           <td><b>1</b></td>
                </table>
<br>
        <p><b>Assignation 2:</b> MIPS excercise</p>
                <p>1. Create a program that adds any two given numbers provided by the user</p>





    .data
	Welcome: .asciiz "/nLets sum two numbers buddy/n"
	result: .asciiz "/nThis is your solve: "
	number1: .asciiz "/nEnter the first number: "
	number2: .asciiz "/nEnter the second number: "
    .text
	main:
	li $v0, 4
	la $a0, Welcome
	syscall
	
	li $v0, 4
	la $a0, number1
	syscall 
	
	li $v0, 5
	syscall
	
	move $t0, $v0
	
	li $v0, 4
	la $a0, number2
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



<br>
        <p>2. Create a program that displays your name</p>

    .data
	name: .asciiz "/nHi, my name is Miguel/n"
    .text
	main:
	li $v0, 4
	la $a0, name
	syscall