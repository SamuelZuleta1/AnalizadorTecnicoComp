# 01 - Analizador léxico de la calculadora


## Output del programa

```
let x = 5;
let y = 10.5;
let z = 0;

/* Operaciones aritmeticas basicas
   con precedencia y agrupacion */
resultado = x + y * 2 - 3 / 4;
otro = (x + y) * (x - y);

// Funciones matematicas y constantes
angulo = sin(pi / 2);
valor_cos = cos(0);
raiz = sqrt(16);
potencia = 2 ^ 8;
val_log = log(100);
val_ln = ln(2);
valor_abs = abs(7);

/* Uso de modulo, ambas formas */
resto1 = 10 mod 3;
resto2 = 10 % 3;

// Comparaciones para el condicional
if (x >= y)
   then max = x
else
   max = y;

// Reutilizar el ultimo resultado
total = ans + 1;

// Impresion del resultado
print(total);
LexToken(LET,'let',2,1)
LexToken(ID,'x',2,5)
LexToken(EQUAL,'=',2,7)
LexToken(NUMBER,5.0,2,9)
LexToken(SEMICOLON,';',2,10)
LexToken(LET,'let',3,12)
LexToken(ID,'y',3,16)
LexToken(EQUAL,'=',3,18)
LexToken(NUMBER,10.5,3,20)
LexToken(SEMICOLON,';',3,24)
LexToken(LET,'let',4,26)
LexToken(ID,'z',4,30)
LexToken(EQUAL,'=',4,32)
LexToken(NUMBER,0.0,4,34)
LexToken(SEMICOLON,';',4,35)
LexToken(ID,'resultado',8,108)
LexToken(EQUAL,'=',8,118)
LexToken(ID,'x',8,120)
LexToken(PLUS,'+',8,122)
LexToken(ID,'y',8,124)
LexToken(TIMES,'*',8,126)
LexToken(NUMBER,2.0,8,128)
LexToken(MINUS,'-',8,130)
LexToken(NUMBER,3.0,8,132)
LexToken(DIVIDE,'/',8,134)
LexToken(NUMBER,4.0,8,136)
LexToken(SEMICOLON,';',8,137)
LexToken(ID,'otro',9,139)
LexToken(EQUAL,'=',9,144)
LexToken(LPAREN,'(',9,146)
LexToken(ID,'x',9,147)
LexToken(PLUS,'+',9,149)
LexToken(ID,'y',9,151)
LexToken(RPAREN,')',9,152)
LexToken(TIMES,'*',9,154)
LexToken(LPAREN,'(',9,156)
LexToken(ID,'x',9,157)
LexToken(MINUS,'-',9,159)
LexToken(ID,'y',9,161)
LexToken(RPAREN,')',9,162)
LexToken(SEMICOLON,';',9,163)
LexToken(ID,'angulo',12,204)
LexToken(EQUAL,'=',12,211)
LexToken(SIN,'sin',12,213)
LexToken(LPAREN,'(',12,216)
LexToken(PI,'pi',12,217)
LexToken(DIVIDE,'/',12,220)
LexToken(NUMBER,2.0,12,222)
LexToken(RPAREN,')',12,223)
LexToken(SEMICOLON,';',12,224)
LexToken(ID,'valor_cos',13,226)
LexToken(EQUAL,'=',13,236)
LexToken(COS,'cos',13,238)
LexToken(LPAREN,'(',13,241)
LexToken(NUMBER,0.0,13,242)
LexToken(RPAREN,')',13,243)
LexToken(SEMICOLON,';',13,244)
LexToken(ID,'raiz',14,246)
LexToken(EQUAL,'=',14,251)
LexToken(SQRT,'sqrt',14,253)
LexToken(LPAREN,'(',14,257)
LexToken(NUMBER,16.0,14,258)
LexToken(RPAREN,')',14,260)
LexToken(SEMICOLON,';',14,261)
LexToken(ID,'potencia',15,263)
LexToken(EQUAL,'=',15,272)
LexToken(NUMBER,2.0,15,274)
LexToken(POWER,'^',15,276)
LexToken(NUMBER,8.0,15,278)
LexToken(SEMICOLON,';',15,279)
LexToken(ID,'val_log',16,281)
LexToken(EQUAL,'=',16,289)
LexToken(LOG,'log',16,291)
LexToken(LPAREN,'(',16,294)
LexToken(NUMBER,100.0,16,295)
LexToken(RPAREN,')',16,298)
LexToken(SEMICOLON,';',16,299)
LexToken(ID,'val_ln',17,301)
LexToken(EQUAL,'=',17,308)
LexToken(LN,'ln',17,310)
LexToken(LPAREN,'(',17,312)
LexToken(NUMBER,2.0,17,313)
LexToken(RPAREN,')',17,314)
LexToken(SEMICOLON,';',17,315)
LexToken(ID,'valor_abs',18,317)
LexToken(EQUAL,'=',18,327)
LexToken(ABS,'abs',18,329)
LexToken(LPAREN,'(',18,332)
LexToken(NUMBER,7.0,18,333)
LexToken(RPAREN,')',18,334)
LexToken(SEMICOLON,';',18,335)
LexToken(ID,'resto1',21,372)
LexToken(EQUAL,'=',21,379)
LexToken(NUMBER,10.0,21,381)
LexToken(MOD,'mod',21,384)
LexToken(NUMBER,3.0,21,388)
LexToken(SEMICOLON,';',21,389)
LexToken(ID,'resto2',22,391)
LexToken(EQUAL,'=',22,398)
LexToken(NUMBER,10.0,22,400)
LexToken(PERCENT,'%',22,403)
LexToken(NUMBER,3.0,22,405)
LexToken(SEMICOLON,';',22,406)
LexToken(IF,'if',25,446)
LexToken(LPAREN,'(',25,449)
LexToken(ID,'x',25,450)
LexToken(GREATEREQUAL,'>=',25,452)
LexToken(ID,'y',25,455)
LexToken(RPAREN,')',25,456)
LexToken(THEN,'then',26,461)
LexToken(ID,'max',26,466)
LexToken(EQUAL,'=',26,470)
LexToken(ID,'x',26,472)
LexToken(ELSE,'else',27,474)
LexToken(ID,'max',28,482)
LexToken(EQUAL,'=',28,486)
LexToken(ID,'y',28,488)
LexToken(SEMICOLON,';',28,489)
LexToken(ID,'total',31,526)
LexToken(EQUAL,'=',31,532)
LexToken(ANS,'ans',31,534)
LexToken(PLUS,'+',31,538)
LexToken(NUMBER,1.0,31,540)
LexToken(SEMICOLON,';',31,541)
LexToken(PRINT,'print',34,571)
LexToken(LPAREN,'(',34,576)
LexToken(ID,'total',34,577)
LexToken(RPAREN,')',34,582)
LexToken(SEMICOLON,';',34,583)
```
