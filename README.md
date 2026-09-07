# UnicodeIcons

A collection of Unicode symbols and emoji constants for C# desktop applications (WinForms, WPF, etc.).

---

Türkçe
======

## Hakkında

Bu repo, C# masaüstü uygulamalarında (Windows Forms, WPF, vb.) kullanılmak üzere düzenlenmiş Unicode sembol ve emoji sabitlerini içerir. `UISymbols` sınıfındaki `public const string` alanlarını doğrudan UI öğelerinizin `Text`/`Content` özelliklerinde kullanabilirsiniz.

## Kurulum

1. `UISymbols.cs` dosyasını projenize ekleyin (ör. `Helpers` veya `Properties` klasörü).
2. Dosyanın UTF-8 olarak kaydedildiğinden emin olun; aksi halde bazı emoji/simgeler bozulabilir.
3. Gerekirse uygun bir namespace ekleyin (`MyApp.UI` gibi).

## Kullanım Örnekleri

1) Windows Forms — Kod içinde

```csharp
// Doğrudan sabitleri kullanma
label1.Text = UISymbols.Settings + " Ayarlar";

// C# 6+ ile using static kullanımı
// using static YourNamespace.UISymbols;
// label1.Text = Settings + " Ayarlar";
```

2) WPF — Code-behind

```csharp
myTextBlock.Text = UISymbols.Search + " Ara";
```

3) WPF — XAML (x:Static ile)

```xml
<!-- XAML içinde kullanmak için: -->
<!-- xmlns:ui="clr-namespace:YourNamespace" -->
<TextBlock Text="{x:Static ui:UISymbols.Search}" />
```

4) Konsol uygulaması

```csharp
Console.WriteLine($"{UISymbols.Star} Favorilere eklendi");
```

5) Unicode kaçış dizisi veya kod kullanımı

```csharp
// Unicode kaçış dizisi
label1.Text = "\u2605"; // "★"

// Karakter koduyla
char star = (char)0x2605;
label1.Text = star.ToString();
```

## Yazı Tipi ve Platform Desteği

- Emoji ve bazı gelişmiş semboller işletim sistemi ve yazı tipine bağlı olarak farklı görünür veya hiç görünmeyebilir.
- Windows için "Segoe UI Symbol" veya "Segoe UI Emoji" gibi yazı tipleri genelde daha iyi destek sağlar.
- Belirli bir sembol görünmüyorsa alternatif bir yazı tipi ya da ikon (resim) kullanmayı değerlendirin.

## Örnek Semboller (küçük seçki)

- Yönler: ← ↑ → ↓ (U+2190–2193)
- Durum/işaretler: ✔ ✖ ⚠ (U+2714, U+2716, U+26A0)
- Posta/Çağrı: ✉ ✆ ☎ (U+2709, U+260E)
- Emoji: 💾 🖨️ 🔍 ⭐

## Katkıda Bulunma

Katkılarınızı bekleriz — yeni sembol önerileri, kategorilendirme veya hata düzeltmeleri için lütfen issue açın veya pull request gönderin. Eklediğiniz semboller için kısa bir açıklama ve kullanım örneği ekleyin.

---

English
=======

## About

This repository provides Unicode symbol and emoji constants intended for use in C# desktop applications (Windows Forms, WPF, etc.). The `UISymbols` class exposes `public const string` fields that you can reference directly in UI element `Text`/`Content` properties.

## Installation

1. Add the `UISymbols.cs` file to your project (e.g. in a `Helpers` or `Properties` folder).
2. Ensure the file is saved in UTF-8 encoding so emoji and symbols render correctly.
3. Add or adjust the namespace if necessary (e.g. `MyApp.UI`).

## Usage Examples

1) Windows Forms — in code

```csharp
// Use the constants directly
label1.Text = UISymbols.Settings + " Settings";

// Or with using static (C# 6+):
// using static YourNamespace.UISymbols;
// label1.Text = Settings + " Settings";
```

2) WPF — code-behind

```csharp
myTextBlock.Text = UISymbols.Search + " Search";
```

3) WPF — XAML (x:Static)

```xml
<!-- In XAML: -->
<!-- xmlns:ui="clr-namespace:YourNamespace" -->
<TextBlock Text="{x:Static ui:UISymbols.Search}" />
```

4) Console application

```csharp
Console.WriteLine($"{UISymbols.Star} Added to favorites");
```

5) Using Unicode escapes or character codes

```csharp
// Unicode escape
label1.Text = "\u2605"; // "★"

// Using a character code
char star = (char)0x2605;
label1.Text = star.ToString();
```

## Font & Platform Support

- Emoji and some symbols may render differently or not at all depending on OS and font.
- On Windows, fonts like "Segoe UI Symbol" or "Segoe UI Emoji" generally provide better coverage.
- If a symbol doesn't render, consider using an alternate font or an image/icon asset.

## Example Symbols (small sample)

- Arrows/Direction: ← ↑ → ↓ (U+2190–2193)
- Status/Marks: ✔ ✖ ⚠ (U+2714, U+2716, U+26A0)
- Mail/Call: ✉ ✆ ☎ (U+2709, U+260E)
- Emoji: 💾 🖨️ 🔍 ⭐

## Contributing

Please open an issue or submit a pull request with new symbols, categorization improvements, or fixes. Include a short description and usage examples for additions.
