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
        Console.WriteLine(Bilgiler());
    }

    private StringBuilder Bilgiler()
    {
        return new StringBuilder()
            .AppendLine($"Ad = {_umutd.Ad}")
            .AppendLine($"Tür = {_umutd.Tur}")
            .AppendLine($"Ünvan = {_umutd.Unvan}")
            .AppendLine($"Favori Programlama Dili = {_umutd.FavoriProgramlamaDili}");
    }
}

public class Program
{
    private static void Main()
    {
        Kunye kunye = new Kunye(new Ben
        {
            Ad = "Umut D.",
            Unvan = "Lüzumsuz İşler Müdürü",
            FavoriProgramlamaDili = "C#"
        });
        kunye.Yazdir();
    }
}
```

![Github Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=umut-d&layout=compact&hide=html)
