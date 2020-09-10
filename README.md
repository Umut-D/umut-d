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
        // Diğer iki ayaklı cisimlerin aksine 'İnsan' olduğumu belirtme gereği duydum
        return new Ben {Tur = "İnsan", FavoriDil = "C#", Unvan = "Lüzumsuz İşler Müdürü"};
    }

    public void Yaz()
    {
        var kisi = Bilgi();

        Console.WriteLine($"Ad = {kisi.Tur}");
        Console.WriteLine($"Favori Programlama Dili = {kisi.FavoriDil}");
        Console.WriteLine($"Ünvan = {kisi.Unvan}");
    }
}
```

![Github Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=umut-d&layout=compact&hide=html)
