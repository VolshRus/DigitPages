Часто нужно вывести значение переменной где-то посередине текста. Можно написать так:
```cs
string itemName = "Стрелы холода";
int price = 15;
int count = 20;
Сonsole.Write(itemName);
Console.Write(" стоят по ");
Console.Write(price);
Console.Write(" монет. Всего ");
Console.WriteLine(count);
```
выведет:
```
Стрелы холода стоят по 15 монет. Всего: 20
```
Но это неудобно, слишком много методов. Есть способ сократить запись - использовать сложение.
```csharp
string itemName = "Стрелы холода";
int price = 15;
int count = 20;
Сonsole.WriteLine(itemName + " стоят по " + price + " монет. Всего " + count);
```
Уже лучше, но читать все равно сложно. Поэтому самый правильный способ:
1. Перед кавычками, в которых задается текст, нужно поставить `$`.
1. Имя переменной пишется прямо в тексте, но оборачивается в фигурные скобки.
```csharp
string itemName = "Стрелы холода";
int price = 15;
int count = 20;
Сonsole.WriteLine($"{itemName} стоят по {price} монет. Всего {count}.");
Сonsole.WriteLine($"Общая стоимость: {price * count}");
```
