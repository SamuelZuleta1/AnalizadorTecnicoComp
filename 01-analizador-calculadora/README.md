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
raiz = sqrt(16);
potencia = 2 ^ 8;
val_exp = exp(1);
area = pi * 2 ^ 2;
val_e = e * 2;

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
LexToken(ID,'raiz',12,204)
LexToken(EQUAL,'=',12,209)
LexToken(SQRT,'sqrt',12,211)
LexToken(LPAREN,'(',12,215)
LexToken(NUMBER,16.0,12,216)
LexToken(RPAREN,')',12,218)
LexToken(SEMICOLON,';',12,219)
LexToken(ID,'potencia',13,221)
LexToken(EQUAL,'=',13,230)
LexToken(NUMBER,2.0,13,232)
LexToken(POWER,'^',13,234)
LexToken(NUMBER,8.0,13,236)
LexToken(SEMICOLON,';',13,237)
LexToken(ID,'val_exp',14,239)
LexToken(EQUAL,'=',14,247)
LexToken(EXP,'exp',14,249)
LexToken(LPAREN,'(',14,252)
LexToken(NUMBER,1.0,14,253)
LexToken(RPAREN,')',14,254)
LexToken(SEMICOLON,';',14,255)
LexToken(ID,'area',15,257)
LexToken(EQUAL,'=',15,262)
LexToken(PI,'pi',15,264)
LexToken(TIMES,'*',15,267)
LexToken(NUMBER,2.0,15,269)
LexToken(POWER,'^',15,271)
LexToken(NUMBER,2.0,15,273)
LexToken(SEMICOLON,';',15,274)
LexToken(ID,'val_e',16,276)
LexToken(EQUAL,'=',16,282)
LexToken(E,'e',16,284)
LexToken(TIMES,'*',16,286)
LexToken(NUMBER,2.0,16,288)
LexToken(SEMICOLON,';',16,289)
LexToken(ID,'resto1',19,326)
LexToken(EQUAL,'=',19,333)
LexToken(NUMBER,10.0,19,335)
LexToken(MOD,'mod',19,338)
LexToken(NUMBER,3.0,19,342)
LexToken(SEMICOLON,';',19,343)
LexToken(ID,'resto2',20,345)
LexToken(EQUAL,'=',20,352)
LexToken(NUMBER,10.0,20,354)
LexToken(PERCENT,'%',20,357)
LexToken(NUMBER,3.0,20,359)
LexToken(SEMICOLON,';',20,360)
LexToken(IF,'if',23,400)
LexToken(LPAREN,'(',23,403)
LexToken(ID,'x',23,404)
LexToken(GREATEREQUAL,'>=',23,406)
LexToken(ID,'y',23,409)
LexToken(RPAREN,')',23,410)
LexToken(THEN,'then',24,415)
LexToken(ID,'max',24,420)
LexToken(EQUAL,'=',24,424)
LexToken(ID,'x',24,426)
LexToken(ELSE,'else',25,428)
LexToken(ID,'max',26,436)
LexToken(EQUAL,'=',26,440)
LexToken(ID,'y',26,442)
LexToken(SEMICOLON,';',26,443)
LexToken(ID,'total',29,480)
LexToken(EQUAL,'=',29,486)
LexToken(ANS,'ans',29,488)
LexToken(PLUS,'+',29,492)
LexToken(NUMBER,1.0,29,494)
LexToken(SEMICOLON,';',29,495)
LexToken(PRINT,'print',32,525)
LexToken(LPAREN,'(',32,530)
LexToken(ID,'total',32,531)
LexToken(RPAREN,')',32,536)
LexToken(SEMICOLON,';',32,537)
```
