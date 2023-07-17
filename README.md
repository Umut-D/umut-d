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
    private readonly Ben _umutD;
    public string Bilgiler => $"Ad = {_umutD.Ad} \n"
                            + $"Tür = {_umutD.Tur} \n"
                            + $"Ünvan = {_umutD.Unvan} \n"
                            + $"Favori Programlama Dili = {_umutD.FavoriProgramlamaDili}";

    public Kunye(Ben umutD)
    {
        _umutD = umutD;
    }
}

public class Program
{
    private void Main()
    {
        Kunye kunye = new Kunye(new Ben
        {
            Ad = "Umut D.",
            Unvan = "Lüzumsuz İşler Müdürü",
            FavoriProgramlamaDili = "C#"
        });

        Console.WriteLine(kunye.Bilgiler);

        Console.Read();
    }
}
```

![Github Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=umut-d&layout=compact&hide=html)
