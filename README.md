# Expense Tracker

## Popis projektu

Expense Tracker je desktopová aplikace vytvořená v jazyce C# pomocí technologie Windows Forms a databáze SQLite. Aplikace slouží k evidenci a správě osobních výdajů. Uživatel může zaznamenávat jednotlivé výdaje, ukládat je do databáze, upravovat je, mazat a následně analyzovat pomocí přehledných statistik a grafů.

Cílem projektu bylo vytvořit jednoduchý, přehledný a uživatelsky přívětivý nástroj pro sledování osobních financí a zároveň demonstrovat práci s databází, grafickým uživatelským rozhraním, vizualizací dat a exportem dat do různých formátů.

## Použité technologie

* C#
* Windows Forms (.NET Framework)
* SQLite
* System.Data.SQLite
* iTextSharp (export PDF)
* DataGridView
* Chart Control

## Hlavní funkce aplikace

### Správa výdajů

Aplikace umožňuje:

* Přidání nového výdaje
* Úpravu existujícího výdaje
* Smazání výdaje
* Zobrazení všech uložených výdajů

Každý výdaj obsahuje:

* Datum
* Kategorii
* Částku
* Popis

### Databáze SQLite

Veškerá data jsou ukládána do lokální databáze SQLite. Díky tomu jsou data zachována i po ukončení aplikace a není potřeba žádný externí databázový server.

### Kategorie výdajů

Při vytváření výdaje si uživatel vybírá kategorii z předdefinovaného seznamu:

* Jídlo
* Auto
* Bydlení
* Zábava
* Oblečení
* Ostatní

Použití ComboBoxu zabraňuje zadávání neplatných nebo nekonzistentních kategorií.

### Vyhledávání

Aplikace umožňuje rychlé vyhledávání v uložených výdajích podle:

* Kategorie
* Popisu

Vyhledávání probíhá v reálném čase při zadávání textu.

### Statistiky

Aplikace automaticky počítá:

* Celkovou částku všech výdajů
* Součet výdajů za aktuální měsíc

Tyto informace poskytují uživateli rychlý přehled o jeho finanční situaci.

### Grafické zobrazení dat

Výdaje jsou vizualizovány pomocí grafů.

Uživatel si může zvolit:

* Koláčový graf
* Sloupcový graf

Grafy zobrazují součet výdajů podle jednotlivých kategorií.

### Export dat

Aplikace umožňuje exportovat data do:

#### CSV

Data lze uložit do CSV souboru a následně otevřít například v programu Microsoft Excel.

#### PDF

Aplikace dokáže vytvořit PDF report obsahující:

* Seznam výdajů
* Celkovou utracenou částku

### Tmavý režim

Aplikace obsahuje přepínatelný tmavý režim.

Uživatel si může zvolit mezi:

* Světlým režimem
* Tmavým režimem

Zvolený režim je uložen do databáze a po opětovném spuštění aplikace je automaticky obnoven.

### Ošetření chyb

Aplikace kontroluje správnost zadávaných údajů.

Například:

* Částka musí být číslo
* Nelze uložit neplatné hodnoty

V případě chyby je uživatel informován pomocí dialogového okna.
