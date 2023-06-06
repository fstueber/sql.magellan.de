# Tabelle **ASVTafelKategorien**



## Spalten

Diese Tabelle hat 7 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`ASVTafel`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    

**`Kategorie`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    

**`ASVInhaltetafel`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Position`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`Merkmal`**

:   [`VARCHAR(8)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`PK_ASVTAFELKATEGORIEN`**

:   `Mandant, ID`

    

## Fremdschlüssel

Diese Tabelle hat 2 Fremdschlüssel.

**`FK_ASVTAFELKATEGORIEN_KATEGORIE`**

:   `Kategorie` » [`ASVKategorien (Kuerzel)`](../../tables/asvkategorien) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

    

**`FK_ASVTAFELKAT_INHALTETAFEL`**

:   `ASVInhaltetafel, Mandant` » [`ASVInhaltetafeln (Kuerzel, Mandant)`](../../tables/asvinhaltetafeln) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

    

## Indizes

Diese Ansicht hat 4 Indizes.

**`FK_ASVTAFELKATEGORIEN_ASVTAFEL`**

:   `Mandant, ASVTafel`

    

**`FK_ASVTAFELKATEGORIEN_KATEGORIE`**

:   `Kategorie`

    

**`FK_ASVTAFELKAT_INHALTETAFEL`**

:   `Mandant, ASVInhaltetafel`

    

**`PK_ASVTAFELKATEGORIEN`**

:   `Mandant, ID`

    
