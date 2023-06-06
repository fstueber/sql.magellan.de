# Tabelle **Unterrichtseinheiten**



## Spalten

Diese Tabelle hat 12 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`VeranstaltungNr`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`Klasse`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`Fach`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`Unterrichtsart`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Fachstatus`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Schwerpunkt`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`KursNr`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`Soll`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

    

**`Angleichung`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

    

**`Bemerkung`**

:   [`BLOB subtype text  `](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

    

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`PK_UEINHEITEN`**

:   `Mandant, ID`

    

## Fremdschlüssel

Diese Tabelle hat 4 Fremdschlüssel.

**`FK_UEINHEITEN_FACHSTATUS`**

:   `Fachstatus` » [`Fachstati (Kuerzel)`](../../tables/fachstati) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

    

**`FK_UEINHEITEN_KLASSE`**

:   `Klasse, Mandant` » [`Klassen (ID, Mandant)`](../../tables/klassen) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

    

**`FK_UEINHEITEN_SCHWERPUNKT`**

:   `Schwerpunkt` » [`Fachschwerpunkte (Kuerzel)`](../../tables/fachschwerpunkte) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

    

**`FK_UEINHEITEN_UNTERRICHTSART`**

:   `Unterrichtsart` » [`Unterrichtsarten (Kuerzel)`](../../tables/unterrichtsarten) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

    

## Indizes

Diese Ansicht hat 6 Indizes.

**`FK_UEINHEITEN_FACH`**

:   `Mandant, Fach`

    

**`FK_UEINHEITEN_FACHSTATUS`**

:   `Fachstatus`

    

**`FK_UEINHEITEN_KLASSE`**

:   `Mandant, Klasse`

    

**`FK_UEINHEITEN_SCHWERPUNKT`**

:   `Schwerpunkt`

    

**`FK_UEINHEITEN_UNTERRICHTSART`**

:   `Unterrichtsart`

    

**`PK_UEINHEITEN`**

:   `Mandant, ID`

    
