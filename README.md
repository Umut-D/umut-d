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
    public static void Yazdir(Ben umutd)
    {
        Console.WriteLine(Bilgiler(umutd));
    }

    private static StringBuilder Bilgiler(Ben umutd)
    {
        return new StringBuilder()
            .AppendLine($"Ad = {umutd.Ad}")
            .AppendLine($"Tür = {umutd.Tur}")
            .AppendLine($"Ünvan = {umutd.Unvan}")
            .AppendLine($"Favori Programlama Dili = {umutd.FavoriProgramlamaDili}");
    }
}

public class Program
{
    private static void Main()
    {
        Ben umutd = new Ben
        {
            Ad = "Umut D.",
            Unvan = "Lüzumsuz İşler Müdürü",
            FavoriProgramlamaDili = "C#"
        };

        Kunye.Yazdir(umutd);
    }
}
```

![Github Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=umut-d&layout=compact&hide=html)
