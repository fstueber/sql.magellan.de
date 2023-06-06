# Tabelle **FaecherUnterpunkte**



## Spalten

Diese Tabelle hat 10 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`Kuerzel`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    

**`Schluessel`**

:   [`VARCHAR(15)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`FUBezeichnung`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Thema`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`Position`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`StatistikID`**

:   [`VARCHAR(16)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`GueltigVon`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes)

    

**`GueltigBis`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes)

    

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`PK_FaecherUnterpunkte`**

:   `Mandant, ID`

    

## Fremdschlüssel

Diese Tabelle hat einen Fremdschlüssel.

**`FK_FAECHERUNTERPUNKTE_THEMA`**

:   `Mandant, Thema` » [`FaecherThemen (ID, Mandant)`](../../tables/faecherthemen) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

    

## Indizes

Diese Ansicht hat 6 Indizes.

**`FK_FAECHERUNTERPUNKTE_MANDANTEN`**

:   `Mandant`

    

**`FK_FAECHERUNTERPUNKTE_THEMA`**

:   `Mandant, Thema`

    

**`IDX_FaecherUnterpunkte_Kuerzel`**

:   `Kuerzel`

    

**`IDX_FaecherUnterpunkte_Mandant`**

:   `Mandant`

    

**`IDX_FaecherUnterpunkte_Thema`**

:   `Mandant, Thema`

    

**`PK_FaecherUnterpunkte`**

:   `Mandant, ID`

    
