```csharp
public class Ben
    {
        public string Ad { get; set; }
        public string Favori { get; set; }
        public string Unvan { get; set; }
    }

    public class Aciklama
    {
        private Ben Bilgi()
        {
            return new Ben {Ad = "Umut D.", Favori = "C#", Unvan = "Lüzumsuz İşler Müdürü"};
        }

        public void Yaz()
        {
            Ben kisi = Bilgi();

            Console.WriteLine($"Ad = {kisi.Ad}");
            Console.WriteLine($"Favori Programlama Dili = {kisi.Favori}");
            Console.WriteLine($"Ünvan = {kisi.Unvan}");
        }
```

![Github Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=umut-d&layout=compact&hide=html)

![Github Stats](https://readmestats.vercel.app/api?username=umut-d&show_icons=true&title_color=333&icon_color=d43111&count_private=true&include_all_commits=true)
