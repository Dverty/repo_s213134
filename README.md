## Temat i struktura zbioru danych         

Przygotowany zbiór danych reprezentuje **listę zakupów**. Całość składa się z tytułu listy oraz zestawu produktów, z których każdy opisany jest za pomocą czterech atrybutów:
- **Kategoria** – np. nabiał, pieczywo, owoce,
- **Nazwa** – nazwa konkretnego produktu,
- **Cena** – wartość numeryczna produktu,
- **Jednostka miary** – sposób określania ilości (`kg` lub `sztuki`).

Dane te zostały zapisane w trzech różnych formatach: **XML** (wraz ze schematem **XSD**), **JSON** oraz **CSV**. Całe repo zostało wykonane używając terminala na
Ubuntu w języku **Bash** i zapisane używając komend git na GitHubie.

---

## Cechy poszczególnych rozwiązań i różnice w zapisie

### 1. XML i XSD         
- **Struktura znaczników:** Wykorzystuje system zagnieżdżonych znaczników (tagów otwierających `<tag>` i zamykających `</tag>`), które definiują hierarchię danych.
- **Walidacja schematem (XSD):** Do pliku dołączono osobny plik `.xsd`, który narzuca ścisłą strukturę dokumentu.
Określa on wymaganą kolejność elementów oraz typy danych.

### 2. JSON         
- **Składnia klamrowa:** Opiera się na systemie nawiasów klamrowych `{}` (do tworzenia obiektów) oraz kwadratowych `[]` (do tworzenia list/tablic), co czyni go bardziej czytelnym 
 w mojej opinii i pozwala na łatwiejsze przetwarzanie danych w aplikacjach i skryptach.
- **Rodzaj zapisu:** Wewnątrz obiektów dane zapisywane są w formie `"klasa": "wartość"` w kolejności, ułatwia to zapis w porównaniu do XML.

### 3. CSV         
- **Format:** Najprostsza, płaska forma zapisu danych tekstowych, w której kolejne wartości oddzielane są przecinkami lub średnikami.
- **Nagłówek kolumn:** Pierwszy wiersz pliku określa nazwy kolumn, do których przyporządkowane są wartości z kolejnych wierszy.

---

## Jak czytać i otwierać pliki?         

1. **Plik CSV (`*.csv`)** – można otworzyć w dowolnym edytorze tekstu lub zaimportować bezpośrednio do
 **LibreOffice Calc** albo **Microsoft Excel**, gdzie dane ułożą się w kolumnach.
2. **Plik JSON (`*.json`)** – najlepiej otwierać w edytorach kodu lub w przeglądarce internetowej, która pomaga czytać strukturę obiektów i tablic.
3. **Plik XML (`*.xml`) oraz XSD (`*.xsd`)** – można podejrzeć w przeglądarce internetowej lub edytorze tekstu.
