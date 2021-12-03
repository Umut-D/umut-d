```csharp
public class Ben
{
    public string Ad { get; set; }
    public string Tur => "İnsan"; // Diğer iki ayaklıların aksine 'İnsan' olduğumu belirtme gereği duydum
    public string Unvan { get; set; }
    public string FavoriProgramlamaDili { get; set; }
}

public class Kunye
{
    private readonly Ben _umutd;

    public Kunye(Ben umutd)
    {
        _umutd = umutd;
    }

    public void Yazdir()
    {
        StringBuilder bilgiler = new StringBuilder()
        .AppendLine($"Ad = _umutd}")
        .AppendLine($"Tür = {_umutd.Tur}")
        .AppendLine($"Ünvan = {_umutd.Unvan}")
        .AppendLine($"Favori Programlama Dili = {_umutd.FavoriProgramlamaDili}");
            
        Console.WriteLine(bilgiler);
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
        kunye.Yazdir();

        Console.Read();
    }
}
```

![Github Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=umut-d&layout=compact&hide=html)
