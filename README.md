# UnicodeIcons

A collection of Unicode symbols and emoji constants for C# desktop applications (WinForms, WPF, etc.).

# Unicode Icons Reference

This document organizes the provided C# icon constants into clean, readable Markdown tables categorized by their respective classes and themes.

## 1. Status
| Icon Name | Symbol | Code/Character |
| :--- | :---: | :--- |
| `Success` | ✔ | `"\u2714"` |
| `Error` | ✖ | `"\u2716"` |
| `Warning` | ⚠ | `"\u26A0"` |
| `Info` | ℹ | `"\u2139"` |
| `Lock` | 🔒 | `"\U0001F512"` |
| `Unlock` | 🔓 | `"\U0001F513"` |

## 2. UI
| Icon Name | Symbol | Code/Character |
| :--- | :---: | :--- |
| `Settings` | ⚙ | `"\u2699"` |
| `Search` | 🔍 | `"\U0001F50D"` |
| `Save` | 💾 | `"\U0001F4BE"` |
| `Folder` | 📁 | `"\U0001F4C1"` |
| `File` | 📄 | `"\U0001F4C4"` |
| `Trash` | 🗑 | `"\U0001F5D1"` |
| `Edit` | ✏ | `"\u270F"` |
| `Home` | 🏠 | `"\U0001F3E0"` |

## 3. Ratings (Favori / Değerlendirme)
| Icon Name | Symbol | Code/Character |
| :--- | :---: | :--- |
| `Star` | ★ | `"\u2605"` |
| `Heart` | ❤ | `"\u2764"` |

## 4. Media (Medya Kontrolleri)
| Icon Name | Symbol | Code/Character |
| :--- | :---: | :--- |
| `Play` | ▶ | `"\u25B6"` |
| `Pause` | ⏸ | `"\u23F8"` |
| `Stop` | ⏹ | `"\u23F9"` |
| `Refresh` | 🔄 | `"\U0001F504"` |

## 5. Arrows (Oklar)
| Icon Name | Symbol | Code/Character |
| :--- | :---: | :--- |
| `Right` | ➔ | `"\u2794"` |
| `Left` | ⬅ | `"\u2B05"` |
| `Up` | ⬆ | `"\u2B06"` |
| `Down` | ⬇ | `"\u2B07"` |

## 6. Communication (Kullanıcı & İletişim)
| Icon Name | Symbol | Code/Character |
| :--- | :---: | :--- |
| `User` | 👤 | `"\U0001F464"` |
| `Users` | 👥 | `"\U0001F465"` |
| `Mail` | ✉ | `"\u2709"` |
| `Phone` | 📞 | `"\U0001F4DE"` |
| `Bell` | 🔔 | `"\U0001F514"` |
| `Eye` | 👁 | `"\U0001F441"` |
| `EyeClosed` | 🙈 | `"\U0001F648"` |

## 7. Data (Dosya & Veri)
| Icon Name | Symbol | Code/Character |
| :--- | :---: | :--- |
| `Attachment` | 📎 | `"\U0001F4CE"` |
| `Link` | 🔗 | `"\U0001F517"` |
| `Database` | 🗄 | `"\U0001F5C4"` |
| `Filter` | 🧹 | `"\U0001F9F9"` |
| `Tag` | 🏷 | `"\U0001F3F7"` |
| `Calendar` | 📅 | `"\U0001F4C5"` |
| `Clock` | 🕒 | `"\U0001F552"` |

## 8. Network (Ağ & Donanım)
| Icon Name | Symbol | Code/Character |
| :--- | :---: | :--- |
| `Wifi` | 📶 | `"\U0001F4F6"` |
| `Globe` | 🌐 | `"\U0001F310"` |
| `Server` | 🖥 | `"\U0001F5A5"` |
| `Terminal` | 💻 | `"\U0001F4BB"` |
| `Signal` | 📡 | `"\U0001F4E1"` |

## 9. Actions (Onay, İşlem & Değerlendirme)
| Icon Name | Symbol | Code/Character |
| :--- | :---: | :--- |
| `CheckMark` | ✅ | `"\u2705"` |
| `CrossMark` | ❌ | `"\u274C"` |
| `Question` | ❓ | `"\u2753"` |
| `Exclamation` | ❗ | `"\u2757"` |
| `Plus` | ➕ | `"\u2795"` |
| `Minus` | ➖ | `"\u2796"` |
| `ThumbsUp` | 👍 | `"\U0001F44D"` |
| `ThumbsDown` | 👎 | `"\U0001F44E"` |

## 10. Navigation (Yönler & Arayüz Navigasyonu)
| Icon Name | Symbol | Code/Character |
| :--- | :---: | :--- |
| `FastForward` | ⏩ | `"\u23E9"` |
| `Rewind` | ⏪ | `"\u23EA"` |
| `Expand` | ⤢ | `"\u2922"` |
| `Collapse` | ⤡ | `"\u2921"` |
| `Menu` | ☰ | `"\u2630"` |
| `MoreHorizontal` | ⋯ | `"\u22EF"` |
| `MoreVertical` | ⋮ | `"\u22EE"` |


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
