```csharp
public class Ben
{
    public string Ad { get; set; }
    public string Tur => "İnsan"; // Diğer iki ayaklıların aksine 'İnsan' olduğumu belirtme gereği duydum
    public string FavoriProgramlamaDili { get; set; }
    public string Unvan { get; set; }
}

public class Kunye
{
    private readonly Ben _ben;

    public Kunye(Ben ben)
    {
        _ben = ben;
    }

    public void Yaz()
    {
        StringBuilder banaDair = new StringBuilder();
        banaDair.AppendLine($"Ad = {_ben.Ad}")
            .AppendLine($"Tür = {_ben.Tur}")
            .AppendLine($"Favori Programlama Dili = {_ben.FavoriProgramlamaDili}")
            .AppendLine($"Ünvan = {_ben.Unvan}");

        Console.WriteLine(banaDair);
    }
}


public class Program
{
    private static void Main()
    {
        Ben umutd = new Ben
        {
            Ad = "Umut D.",
            FavoriProgramlamaDili = "C#",
            Unvan = "Lüzumsuz İşler Müdürü"
        };

        Kunye kunye = new Kunye(umutd);
        kunye.Yaz();

        Console.Read();
    }
}
```

![Github Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=umut-d&layout=compact&hide=html)
