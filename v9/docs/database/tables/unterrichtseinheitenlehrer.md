# Tabelle **UnterrichtseinheitenLehrer**



## Spalten

Diese Tabelle hat 7 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`Unterrichtseinheit`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`Lehrer`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`Ist`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

    

**`Bemerkung`**

:   [`BLOB subtype text  `](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

    

**`Gruppenunterricht`**

:   [`CHAR(1) `](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`PK_UEINHEITENLEHRER`**

:   `Mandant, ID`

    

## Fremdschlüssel

Diese Tabelle hat einen Fremdschlüssel.

**`FK_UEINHEITENLEHRER_UEINHEIT`**

:   `Mandant, Unterrichtseinheit` » [`Unterrichtseinheiten (ID, Mandant)`](../../tables/unterrichtseinheiten) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

    

## Indizes

Diese Ansicht hat 3 Indizes.

**`FK_UEINHEITENLEHRER_LEHRER`**

:   `Mandant, Lehrer`

    

**`FK_UEINHEITENLEHRER_UEINHEIT`**

:   `Mandant, Unterrichtseinheit`

    

**`PK_UEINHEITENLEHRER`**

:   `Mandant, ID`

    
