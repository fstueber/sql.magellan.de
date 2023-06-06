# Tabelle **KlassenbuchKlassen**



## Spalten

Diese Tabelle hat 5 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`Klassenbucheintrag`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`Klasse`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`BlockNr`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Fach`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`PK_KLASSENBUCHKLASSEN`**

:   `Mandant, Klassenbucheintrag, Klasse`

    

## Fremdschlüssel

Diese Tabelle hat einen Fremdschlüssel.

**`FK_KBK_KLASSE`**

:   `Klasse, Mandant` » [`Klassen (ID, Mandant)`](../../tables/klassen) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

    

## Indizes

Diese Ansicht hat 3 Indizes.

**`FK_KBK_EINTRAG`**

:   `Mandant, Klassenbucheintrag`

    

**`FK_KBK_KLASSE`**

:   `Mandant, Klasse`

    

**`PK_KLASSENBUCHKLASSEN`**

:   `Mandant, Klassenbucheintrag, Klasse`

    
