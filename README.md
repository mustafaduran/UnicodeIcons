# UnicodeIcons

Aşağıdaki dosya, C# masaüstü uygulamalarında (Windows Forms, WPF, vb.) kullanılmak üzere Unicode simgeleri/emoji sabitleri sağlar. Bu repo küçük ve tek dosyalı bir koleksiyon içerir: `UISymbols.cs`.

## Kısa Açıklama
`UISymbols` sınıfı içinde tanımlı `public const string` alanları, simge karakterlerini temsil eder. Bu sabitleri uygulama arayüzünüzde doğrudan kullanabilirsiniz.

## Kurulum
- En basit yol: `UISymbols.cs` dosyasını projenize ekleyin (ör. `Properties` veya `Helpers` klasörüne).
- Dosyanın UTF-8 ile kaydedildiğinden emin olun; emoji ve Unicode karakterleri doğru görünmesi için bu önemlidir.

## Kullanım Örnekleri
Aşağıdaki örnekler, `UISymbols` sınıfının global ad alanında yer aldığı varsayımıyla verilmiştir. Eğer `UISymbols` bir namespace içindeyse (`MyApp.UI` gibi), uygun `using` ifadesini ekleyin veya tam yol kullanın (`MyApp.UI.UISymbols.Settings`).

1) Windows Forms (kod ile):

```csharp
// doğrudan referans
label1.Text = UISymbols.Settings + " Ayarlar";

// veya using static ile (C# 6+):
// using static UISymbols;
// label1.Text = Settings + " Ayarlar";
```

2) WPF (kod-behind):

```csharp
// TextBlock örneği
myTextBlock.Text = UISymbols.Search + " Ara";
```

3) WPF XAML (x:Static kullanımı — UISymbols bir namespace içindeyse):

```xml
<!-- XAML içinde kullanmak için: -->
<!-- xmlns:ui="clr-namespace:YourNamespace" -->
<TextBlock Text="{x:Static ui:UISymbols.Search}" />
```

4) Konsol uygulaması (örnek):

```csharp
Console.WriteLine($"{UISymbols.Star} Favorilere eklendi");
```

## Dikkat Edilmesi Gerekenler
- Dosya UTF-8 olarak saklanmalıdır. Bazı editörler farklı encoding kullanırsa emoji bozulabilir.
- Eğer sınıf örneklenmemesi gereken sadece sabitler içeriyorsa, `public static class UISymbols` yapmak daha iyidir (şu anki hâli `public partial class UISymbols`).
- Büyük projelerde `UISymbols` için uygun bir namespace eklemeniz tavsiye edilir.

## Örnek nasıl çalışır (Windows Forms kısa demo)

```csharp
using System.Windows.Forms;

public class DemoForm : Form
{
    private Label lbl;

    public DemoForm()
    {
        lbl = new Label { AutoSize = true };
        lbl.Text = UISymbols.Lock + " Güvenli";
        Controls.Add(lbl);
    }
}
```

---

Eğer isterseniz, ben bu README'yi repoya ekledim. Ayrıca dilerseniz `UISymbols.cs` dosyasını önerdiğim şekilde `public static partial class UISymbols` ve bir `namespace` ekleyerek küçük bir PR hazırlayabilirim.