# ARTIFICIAL-INTELLIGENCE-PROGRAMS


### TEMPERATURE CONVERSION

AIM:
To write predicates one converts centigrade temperature to Fahrenheit, other checks if a
temperature is below freezing.

Formula for Centigrade (C) temperatures to Fahrenheit (F) -

F = C * 9 / 5 + 32

PROGRAM
%ex3.pl
%ctof converts C to F
ctof(C,F):-F is C*9/5+32.
%freezing function check the temperature
freezing(F):-F=<32.
OUTPUT:
?- ctof(100,F).
F = 212.
?- freezing(20).
true.
?- freezing(40).
false.

Result: Thus, prolog program to convert centigrade temperature to Fahrenheit is executed successfully


### FACTORIAL OF A NUMBER
AIM: To write prolog program to find Factorial of a Given number.

PROGRAM
%ex4.pl
fact(0,1).
fact(N,F):-N>0,N1 is N-1,fact(N1,F1),F is N * F1.

OUTPUT:
?- fact(5,A).
A = 120 .
?- fact(10,B).
B = 3628800
?- fact(5,720).
false.

Result: Thus, prolog program to find factorial of a number is executed successfully.


### GCD OF TWO NUMBERS
AIM: To write prolog program to find GCD of two Numbers.

PROGRAM
%ex5.pl
gcd(X,X,X).
gcd(X,Y,D):- X < Y,Y1 is Y-X,gcd(X,Y1,D).
gcd(X,Y,D):- Y < X,X1 is X-Y,gcd(X1,Y,D).
OUTPUT:
?- gcd(75,30,B).
B = 15 .
?- gcd(15,60,A).
A = 15 .
?- gcd(75,30,B).
B = 15 .

Result: Thus, prolog program to find GCD of two Numbers is executed Successfully.
