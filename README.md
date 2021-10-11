# mina_reader

Mina Reader is a flutter package for Text Reading and Highlighting.

### Features:
- Auto Scroll Text
- Highlight Text with Color 
- Color Labels names can changable by user
- Make Bold, Italic, Underline of selected text
- Last Read Location saves automatically

### Screens
- Book List
- Sections
- Reader Settings

[Get on pub.dev](https://pub.dev/packages/mina_reader)

<img src="https://raw.githubusercontent.com/yazilimsalcozumler/mina_reader/main/docs/assets/demo.gif" alt="Example Project" />


## How to use

```dart
class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return GetMaterialApp(
      title: 'Flutter Demo',
      home: Scaffold(
        body: BooksScreen(
          title: 'Books',
          booksAssetsFolder: "assets/books/",
          books: [
            Book(
              title: 'Asâ-yı Musa',
              assetFolder: 'asayi_musa',
              sections: [
                Section(
                  title: 'Mukaddimat',
                  fileName: 'mukaddimat.txt',
                ),
                Section(
                    title: 'Birinci Mesele', fileName: 'birinci_mesele.txt'),
                Section(
                  title: 'İkinci Mesele',
                  fileName: 'ikinci_mesele.txt',
                )
              ],
            ),
            Book(
              title: 'Sözler',
              sections: [
                Section(
                  title: 'Birinci Söz',
                  fileName: 'birinci_soz.txt',
                ),
                Section(title: 'İkinci Söz', fileName: 'ikinci_soz.txt'),
                Section(
                  title: 'Üçüncü Söz',
                  fileName: 'ucuncu_soz.txt',
                )
              ],
              assetFolder: 'sozler',
            ),
          ],
        ),
      ),
    );
  }
}
```