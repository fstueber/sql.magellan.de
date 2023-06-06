# Tabelle **SchuelerMedizinAkten**



## Spalten

Diese Tabelle hat 8 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`EnbreaID`**

:   [`VARCHAR(24)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Schueler`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`Datum`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes)

    

**`Behandlung`**

:   [`BLOB subtype text  `](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

    

**`Medikationen`**

:   [`BLOB subtype text  `](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

    

**`Bemerkung`**

:   [`BLOB subtype text  `](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

    

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`PK_SCHUELERMEDIZINAKTEN`**

:   `Mandant, ID`

    

## Indizes

Diese Ansicht hat 2 Indizes.

**`FK_SCHUELERMEDAKT_SCHUELER`**

:   `Mandant, Schueler`

    

**`PK_SCHUELERMEDIZINAKTEN`**

:   `Mandant, ID`

    
