# Tabelle **InventarExemplare**



## Spalten

Diese Tabelle hat 11 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`Inventar`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`GeraeteNr`**

:   [`VARCHAR(15)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Bewegungsart`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`Bewegungsdatum`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes)

    

**`Anzahl`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`Betrag`**

:   [`NUMERIC(18, 4)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes)

    

**`Waehrung`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Lieferant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`Bemerkung`**

:   [`BLOB subtype text  `](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

    

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`PK_INVENTAREXEMPLARE`**

:   `Mandant, ID`

    

## Fremdschlüssel

Diese Tabelle hat 2 Fremdschlüssel.

**`FK_INVENTAREXEMPLARE_LIEFERANT`**

:   `Lieferant` » [`Lieferanten (ID)`](../../tables/lieferanten) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

    

**`FK_INVENTAREXEMPLARE_WAEHRUNG`**

:   `Waehrung` » [`Waehrungen (Kuerzel)`](../../tables/waehrungen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

    

## Indizes

Diese Ansicht hat 4 Indizes.

**`FK_INVENTAREXEMPLARE_INVENTAR`**

:   `Mandant, Inventar`

    

**`FK_INVENTAREXEMPLARE_LIEFERANT`**

:   `Lieferant`

    

**`FK_INVENTAREXEMPLARE_WAEHRUNG`**

:   `Waehrung`

    

**`PK_INVENTAREXEMPLARE`**

:   `Mandant, ID`

    
