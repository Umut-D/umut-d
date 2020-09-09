```csharp
public class Ben
{
    public string Tur { get; set; }
    public string FavoriDil { get; set; }
    public string Unvan { get; set; }
}

public class Aciklama
{
    private Ben Bilgi()
    {
        return new Ben {Tur = "İnsan", FavoriDil = "C#", Unvan = "Lüzumsuz İşler Müdürü"};
    }

    public void Yaz()
    {
        Ben kisi = Bilgi();

        Console.Write($"Ad = {kisi.Tur}"); // Diğer iki ayaklı cisimlerin aksine
        Console.WriteLine($"Favori Programlama Dili = {kisi.FavoriDil}");
        Console.WriteLine($"Ünvan = {kisi.Unvan}");
    }
}
```

![Github Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=umut-d&layout=compact&hide=html)
