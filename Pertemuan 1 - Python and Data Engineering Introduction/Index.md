DATA ENGINEERING WEEK 1
======================

- [A. PENGENALAN PYTHON](#a-pengenalan)
    - [Basic Syntax](#basic-syntax)
      - [Indentasi](#indentasi)
      - [Komentar](#comment)
      - [Print](#print)
    - [Variable](#variable)
      - [Dekralasi](#deklarasi)
      - [Casting](#casting)
      - [Case Sensitive](#case-sensitive)
      - [Type Data Check](#check-type)
     - [String Manipulation](#string-manipulation)
     - [Operator](#operator)
        - [Arithmetic Operator](#arithmetic-operator)
        - [Comparison Operator](#comparison-operator)
        - [Logical Operator](#logical-operator)
     - [Percabangan](#percabangan)
     - [Perulangan](#perulangan)
     - [Collection](#collection)

- [B. QUIZ](#b-quiz)

## A PENGENALAN

###  Basic Syntax
#### Indentasi
Dalam bahasa pemrograman lain Indentasi dalam kode hanya untuk keterbacaan, sedangkan dalam Python sangat penting. Python menggunakan indentasi untuk menunjukkan blok kode.\
***Correct***
```
if 5 > 2:
  print("Five is greater than two!")
```
***Wrong***
```
if 5 > 2:
print("Five is greater than two!")
```
#### Comment
Syntax | Penjelasan
------- | ---------
`# Ini Komentar` | Komentar dimulai dengan # dan sisa baris sebagai komentar
####  Print
Syntax | Penjelasan
------- | ---------
`print("Hello World")` | output "Hello World"
`print(var_x)` | output sesuai nilai dari variabel var_x 

### Variable
#### Deklarasi
  1. Variabel dibuat saat Anda pertama kali memberikan nilai padanya.
  2. Deklarasi variabel tidak perlu diikuti tipe data.
  
Syntax | Penjelasan
------- | ---------
`x = 4` | x adalah variabel bertipe int
`y = "Sally"` | y adalah variabel bertipe string
`z = 'String'` | z adalah variabel bertipe string

  3. Nama variable hanya boleh mengandung ankga(0-9), huruf(A-z) dan Underscore(_)
  4. Nama variable tidak boleh diawali dengan angka
***Legal***
```
_my_var = "John"
myVar = "John"
MYVAR = "John"
myvar2 = "John"
```
***ILegal***
```
2myvar = "John"
my-var = "John"
my var = "John"
```
####  Casting
Jika Anda ingin menentukan tipe data dari suatu variabel, hal ini dapat dilakukan dengan casting.
Syntax | Penjelasan
------- | ---------
`x = str(3)` | x adalah variabel bertipe string '3'
`y = int(3)` | y adalah variabel bertipe int 3
`z = float(3)` | z adalah variabel bertipe float 3.0

#### Case Sensitive
`my_var` != `MY_VAR`\
`var` != `VAr`
####  Check Type
```
x = 3
print(type(x)) 
# hasil nya adalah tipe data dari variabel x (int)
```
### String Manipulation
Aksi | Syntax | Penjelasan
-------- | ------- | ---------
Lower Case | [var].lower() | Mengubah semua karakter pada string menjadi huruf kecil
Upper Case | [var].upper() | Mengubah semua karakter pada string mnejadi huruf besar
Strip | [var].strip(arg) | Menghapus karakter di awal dan diakhir string, default menghapus spasi

### Operator
#### Arithmetic Operator

Operator | Name | Example
-------- | ------- | --------
```
+	| Addition | 	x + y
-	| Subtraction | 	x - y
*	| Multiplication | 	x * y
/	| Division | 	x / y
%	| Modulus	x % y	
**	| Exponentiation	| x ** y	
//	| Floor division |	x // y
```
####  Comparison Operator
Name | Syntax | Keterangan
---------- | -------- | -----------
Equal to | 	a == b | Mengembalikan nilai true jika a ***sama*** dengan b
Not equal to | a != b |	 Mengembalikan nilai true jika a ***tidak sama dengan*** b
Greater than	| a > b |	Mengembalikan true jika a ***lebih dari*** b
Less than	| a < b |	Mengembalikan true jika a ***kurang dari*** b
Less than or equal to	| a <= b	| Mengembalikan true jika a ***kurang dari b*** atau a ***sama dengan*** b
Greater than or equal to | a >= b	| Mengembalikan true jika a ***lebih dari*** b atau a ***sama dengan*** b
#### Logical Operator
Operator | Keterangan | Contoh 
--------- | ---------- | -----------
and | mengembalikan true jika kedua statement true	| x < 5 and  x < 10	
or	| mengembalikan true jika sxalah satu statement true |x < 5 or x < 4	
not	| mengembalikan true jika hasil statement false (dan sebaliknya) | not(x < 5 and x < 10)
### Percabangan
```
a = 200
b = 33
c = 500
if a > b and c > a:
  print("Both conditions are True")
```
### Perulangan
#### For Loops
```
fruits = ["apple", "banana", "cherry"]
for x in fruits:
  print(x)
  if x == "banana":
    break
```
#### While Loops
```
i = 1
while i < 6:
  print(i)
  i += 1
```
### Collection
Data Structure | Ordered |  Mutable |  Constructor | Example
--------- | --------- | --------- | --------- | ---------
List | yes | yes | [ ] or list( ) | [5, 1, 'yes', 4, 1.2]
Tuple | yes | no | ( ) or tuple( ) | (5, 1, 'yes', 4, 1.2
Set | no | yes | { }  or set( ) | {5, 1, 'yes', 4, 1.2}
Dictionary | no | yes | { } or dict( ) | {'name' : 'coder', 'from' : 'IT Telkom Surabaya'}




## B QUIZ



###           Q U I Z     1 
```
name = ['Coder']
name.append('Data Engineering')
print(name[1])  

# A. Coder
# B. Data Engineering
# C. Data
```



###           Q U I Z     2
```
def solve(a):
    a = [3, 6]

a = [1, 5]
print(a)
a = solve(a)
print(a)

# A. [1, 5]   [3, 6]
# B. [1, 5]   1, 5]
# C. [1, 5]   none
```



###           Q U I Z     3
```
myList = ["Data", "Engineering"]
for i in myList :
    myList.append(i.upper())
print(myList)

# A. ["Data", "Engineering", "DATA", "ENGINEERING"]
# B. ["DATA", "ENGINEERING"]
# C. Infinitie Loop
```
