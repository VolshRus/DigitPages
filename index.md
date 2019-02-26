Любая программа состоит из набора действий, **методов**. Позже научимся создавать свои, а пока будем использовать готовые.

Метод `Console.Write()` выводит текст в Консоль. Код:

```csharp 
{% highlight csharp %}
Console.Write("Программирование - это круто!");
internal abstract class BuildType
    {
        public string Title { get; private set; }
        public Money Cost { get; private set; }
        public Money Upkeep { get; private set; }
        public NeedType NeedType { get; private set; }
        public ClientsAmount[] ClientsData { get; private set; }

        public string Description => $"{Title} - {Cost}, обслуживает: {ClientsData.Select(t => t.ToString()).Aggregate((t1, t2) => $"{t1} и {t2}")}";

        protected BuildType(string title, Money cost, Money upkeep, NeedType serviceType, params ClientsAmount[] clientsData)
        {
            Title = title;
            Cost = cost;
            Upkeep = upkeep;
            NeedType = serviceType;
            ClientsData = clientsData;
        }
    }
    {% endhighlight %}
```

выведет:

`Программирование - это круто!`

У любого метода есть **имя** и **параметры**. В примере выше, Console.Write - это имя метода, а текст в скобках - параметр.

## Практика

Напиши программу, которая выводит в Консоль сообщение *Hello, world!*

>Изучая новый язык, любой программист первым делом пишет такую программу. Это традиция, которой уже около 40 лет.
