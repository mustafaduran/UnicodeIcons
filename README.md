# UnicodeIcons

A collection of Unicode symbols and emoji constants for C# desktop applications such as WinForms, WPF, and console apps.

This project provides a simple `UISymbols` class with ready-to-use icon constants that can be displayed in labels, buttons, menus, and text-based UI elements.

## Features

- Ready-to-use Unicode constants for UI scenarios
- Works well with WinForms and WPF
- Easy to use in code or XAML
- Organized by category for quick lookup

## Installation

1. Copy the `UISymbols.cs` file into your project (for example under `Helpers`, `UI`, or `Properties`).
2. Make sure the file is saved as UTF-8.
3. Add the correct namespace if needed.

## Usage Examples

### 1. WinForms

```csharp
label1.Text = UISymbols.Settings + " Settings";
label2.Text = UISymbols.Success + " Success";
button1.Text = UISymbols.Search + " Search";
```

### 2. WPF (code-behind)

```csharp
myTextBlock.Text = UISymbols.Search + " Search";
myButton.Content = UISymbols.Save + " Save";
```

### 3. WPF (XAML)

```xml
<TextBlock Text="{x:Static ui:UISymbols.Search}" />
<TextBlock Text="{x:Static ui:UISymbols.Home}" />
```

### 4. Using `using static`

```csharp
using static YourNamespace.UISymbols;

label1.Text = Settings + " Settings";
button1.Text = Star + " Favorites";
```

### 5. Console application

```csharp
Console.WriteLine($"{UISymbols.Star} Added to favorites");
Console.WriteLine($"{UISymbols.CheckMark} Completed");
```

### 6. Unicode escape / code usage

```csharp
label1.Text = "\u2605"; // ★
char star = (char)0x2605;
label1.Text = star.ToString();
```

## Icon Reference

### Status

| Icon Name | Symbol | Unicode / Code |
| :--- | :---: | :--- |
| `Success` | ✔ | `"\u2714"` |
| `Error` | ✖ | `"\u2716"` |
| `Warning` | ⚠ | `"\u26A0"` |
| `Info` | ℹ | `"\u2139"` |
| `Lock` | 🔒 | `"\U0001F512"` |
| `Unlock` | 🔓 | `"\U0001F513"` |

### UI

| Icon Name | Symbol | Unicode / Code |
| :--- | :---: | :--- |
| `Settings` | ⚙ | `"\u2699"` |
| `Search` | 🔍 | `"\U0001F50D"` |
| `Save` | 💾 | `"\U0001F4BE"` |
| `Folder` | 📁 | `"\U0001F4C1"` |
| `File` | 📄 | `"\U0001F4C4"` |
| `Trash` | 🗑 | `"\U0001F5D1"` |
| `Edit` | ✏ | `"\u270F"` |
| `Home` | 🏠 | `"\U0001F3E0"` |

### Ratings

| Icon Name | Symbol | Unicode / Code |
| :--- | :---: | :--- |
| `Star` | ★ | `"\u2605"` |
| `Heart` | ❤ | `"\u2764"` |

### Media Controls

| Icon Name | Symbol | Unicode / Code |
| :--- | :---: | :--- |
| `Play` | ▶ | `"\u25B6"` |
| `Pause` | ⏸ | `"\u23F8"` |
| `Stop` | ⏹ | `"\u23F9"` |
| `Refresh` | 🔄 | `"\U0001F504"` |

### Arrows

| Icon Name | Symbol | Unicode / Code |
| :--- | :---: | :--- |
| `Right` | ➔ | `"\u2794"` |
| `Left` | ⬅ | `"\u2B05"` |
| `Up` | ⬆ | `"\u2B06"` |
| `Down` | ⬇ | `"\u2B07"` |

### Communication

| Icon Name | Symbol | Unicode / Code |
| :--- | :---: | :--- |
| `User` | 👤 | `"\U0001F464"` |
| `Users` | 👥 | `"\U0001F465"` |
| `Mail` | ✉ | `"\u2709"` |
| `Phone` | 📞 | `"\U0001F4DE"` |
| `Bell` | 🔔 | `"\U0001F514"` |
| `Eye` | 👁 | `"\U0001F441"` |
| `EyeClosed` | 🙈 | `"\U0001F648"` |

### Data

| Icon Name | Symbol | Unicode / Code |
| :--- | :---: | :--- |
| `Attachment` | 📎 | `"\U0001F4CE"` |
| `Link` | 🔗 | `"\U0001F517"` |
| `Database` | 🗄 | `"\U0001F5C4"` |
| `Filter` | 🧹 | `"\U0001F9F9"` |
| `Tag` | 🏷 | `"\U0001F3F7"` |
| `Calendar` | 📅 | `"\U0001F4C5"` |
| `Clock` | 🕒 | `"\U0001F552"` |

### Network

| Icon Name | Symbol | Unicode / Code |
| :--- | :---: | :--- |
| `Wifi` | 📶 | `"\U0001F4F6"` |
| `Globe` | 🌐 | `"\U0001F310"` |
| `Server` | 🖥 | `"\U0001F5A5"` |
| `Terminal` | 💻 | `"\U0001F4BB"` |
| `Signal` | 📡 | `"\U0001F4E1"` |

### Actions

| Icon Name | Symbol | Unicode / Code |
| :--- | :---: | :--- |
| `CheckMark` | ✅ | `"\u2705"` |
| `CrossMark` | ❌ | `"\u274C"` |
| `Question` | ❓ | `"\u2753"` |
| `Exclamation` | ❗ | `"\u2757"` |
| `Plus` | ➕ | `"\u2795"` |
| `Minus` | ➖ | `"\u2796"` |
| `ThumbsUp` | 👍 | `"\U0001F44D"` |
| `ThumbsDown` | 👎 | `"\U0001F44E"` |

### Navigation

| Icon Name | Symbol | Unicode / Code |
| :--- | :---: | :--- |
| `FastForward` | ⏩ | `"\u23E9"` |
| `Rewind` | ⏪ | `"\u23EA"` |
| `Expand` | ⤢ | `"\u2922"` |
| `Collapse` | ⤡ | `"\u2921"` |
| `Menu` | ☰ | `"\u2630"` |
| `MoreHorizontal` | ⋯ | `"\u22EF"` |
| `MoreVertical` | ⋮ | `"\u22EE"` |

## Font and Platform Notes

- Some emoji and symbols may render differently depending on the operating system and font.
- On Windows, fonts such as `Segoe UI Symbol` or `Segoe UI Emoji` usually provide better support.
- If a symbol does not appear correctly, consider using a different font or a custom image asset.

## Contributing

Contributions are welcome. If you want to add new symbols, improve categorization, or fix issues, please open an issue or submit a pull request.

## License

This project is provided as-is for educational and development use. Please check the repository license for additional details.
