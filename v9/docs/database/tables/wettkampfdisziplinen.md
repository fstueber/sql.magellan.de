# Tabelle **WettkampfDisziplinen**



## Spalten

Diese Tabelle hat 6 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`Wettkampf`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    

**`Disziplin`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Position`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`Merkmal`**

:   [`VARCHAR(8)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`PK_WETTKAMPFDISZIPLINEN`**

:   `Mandant, ID`

    

## Fremdschlüssel

Diese Tabelle hat einen Fremdschlüssel.

**`FK_WETTKAEMPFE_WETTKAMPF`**

:   `Mandant, Wettkampf` » [`Wettkaempfe (Kuerzel, Mandant)`](../../tables/wettkaempfe) · `ON UPDATE CASCADE` · `ON DELETE CASCADE`

    

## Indizes

Diese Ansicht hat 3 Indizes.

**`FK_WETTKAEMPFE_DISZIPLIN`**

:   `Mandant, Disziplin`

    

**`FK_WETTKAEMPFE_WETTKAMPF`**

:   `Mandant, Wettkampf`

    

**`PK_WETTKAMPFDISZIPLINEN`**

:   `Mandant, ID`

    
