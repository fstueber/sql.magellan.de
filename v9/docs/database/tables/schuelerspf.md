# Tabelle **SchuelerSPF**



## Spalten

Diese Tabelle hat 9 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`Schueler`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`Sportfest`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    

**`Riege`**

:   [`VARCHAR(4)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Punktzahl`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

    

**`Note`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

    

**`UrkundeAm`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes)

    

**`Status`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`Meldungen`**

:   [`BLOB subtype text  `](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

    

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`PK_SCHUELERSPF`**

:   `Mandant, Schueler, Sportfest`

    

## Fremdschlüssel

Diese Tabelle hat einen Fremdschlüssel.

**`FK_SCHUELERSPF_SPORTFEST`**

:   `Mandant, Sportfest` » [`Sportfeste (Kuerzel, Mandant)`](../../tables/sportfeste) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

    

## Indizes

Diese Ansicht hat 3 Indizes.

**`FK_SCHUELERSPF_SCHUELER`**

:   `Mandant, Schueler`

    

**`FK_SCHUELERSPF_SPORTFEST`**

:   `Mandant, Sportfest`

    

**`PK_SCHUELERSPF`**

:   `Mandant, Schueler, Sportfest`

    
