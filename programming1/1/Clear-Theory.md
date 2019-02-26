Метод `Console.Clear()` убирает весь текст в Консоли, который там был на момент его вызова.

Параметров не имеет.

```csharp
Console.WriteLine("Старый текст");
Console.WriteLine("Много-много текста...");
Console.Clear();
Console.WriteLine("Новый текст");
```
Выводет:
```
Новый текст
```
