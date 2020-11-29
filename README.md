```csharp
public class Ben
{
    public string Ad { get; set; }
    public string Tur { get; set; }
    public string FavoriDil { get; set; }
    public string Takim { get; set; }
    public string Unvan { get; set; }
}

public class Aciklama
{
    private Ben Bilgi()
    {
        
        return new Ben
            {
                Ad = "Umut D.",
                Tur = "İnsan", // Diğer iki ayaklı cisimlerin aksine 'İnsan' olduğumu belirtme gereği duydum
                FavoriDil = "C#",
                Takim = "Arsenal",
                Unvan = "Lüzumsuz İşler Müdürü"
            };
    }

    public void Yaz()
    {
        Ben kisi = Bilgi();

        StringBuilder banaDair = new StringBuilder();
        banaDair.AppendLine($"Ad = {kisi.Ad}");
        banaDair.AppendLine($"Tür = {kisi.Tur}");
        banaDair.AppendLine($"Favori Programlama Dili = {kisi.FavoriDil}");
        banaDair.AppendLine($"Tuttuğu Takım = {kisi.Takim}");
        banaDair.AppendLine($"Ünvan = {kisi.Unvan}");

        return banaDair;
    }
}
```

![Github Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=umut-d&layout=compact&hide=html)
