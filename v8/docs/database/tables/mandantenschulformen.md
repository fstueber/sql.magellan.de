# Tabelle **MandantenSchulformen**



## Spalten

Diese Tabelle hat 4 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`Schulform`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    

**`Position`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`Bemerkung`**

:   [`BLOB subtype text  `](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

    

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`PK_MANDANTENSCHULFORMEN`**

:   `Mandant, Schulform`

    

## Fremdschlüssel

Diese Tabelle hat einen Fremdschlüssel.

**`FK_MANDANTENSCHULFORMEN_MANDANT`**

:   `Mandant` » [`Mandanten (ID)`](../../tables/mandanten) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

    

## Indizes

Diese Ansicht hat 3 Indizes.

**`FK_MANDANTENSCHULFORMEN_FORM`**

:   `Schulform`

    

**`FK_MANDANTENSCHULFORMEN_MANDANT`**

:   `Mandant`

    

**`PK_MANDANTENSCHULFORMEN`**

:   `Mandant, Schulform`

    
