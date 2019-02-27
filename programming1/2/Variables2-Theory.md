Чтобы пользоваться переменной, её нужно сначала **объявить** и **инициализировать**.

**Объявить** - значит "забронировать" под нее определенное имя и место в памяти. После уже нельзя будет создать другую переменную с таким именем. 

**Инициализировать** - впервые задать значение. Чаще всего это делают одновременно с объявлением.
```cs
string example = "Пример";
```
Здесь мы объявили переменную с именем example и инициализировали ее значением "Пример". string - это **тип** переменной. От него зависит, какие данные можно записать в переменную и что с ними можно делать.
```cs
string text1 = "Привет";
string text2 = "Пока";
int number1 = 10;
int number2 = 15;
Console.WriteLine(text1 + text2);
Console.WriteLine(number1 + number2);
```
выведет:
```
ПриветПока
15
```
Здесь мы оба раза сложили две переменных. Но в первом случае значения "объединились", а во втором - сложились арифметически. Так получилось, потому что в первом случае мы складывали string, а во втором - int.
>Кстати, операции с разными типами запрещены. Так что text1+number1 выдаст ошибку.
