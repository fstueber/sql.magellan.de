# Tabelle **TransportationLines**



## Spalten

Diese Tabelle hat 8 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`EnbreaID`**

:   [`VARCHAR(24)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`InboundRoute`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`OutboundRoute`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`Operator`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`Code`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    

**`Name`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`PK_TRANSPORTLINES`**

:   `Mandant, ID`

    

## Fremdschlüssel

Diese Tabelle hat 2 Fremdschlüssel.

**`FK_TRANSPORTLINES_OPERATOR`**

:   `Mandant, Operator` » [`Adressen (ID, Mandant)`](../../tables/adressen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

    

**`FK_TRANSPORTLINES_OUTROUTES`**

:   `Mandant, OutboundRoute` » [`TransportationRoutes (ID, Mandant)`](../../tables/transportationroutes) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

    

## Indizes

Diese Ansicht hat 4 Indizes.

**`FK_TRANSPORTLINES_INROUTES`**

:   `Mandant, InboundRoute`

    

**`FK_TRANSPORTLINES_OPERATOR`**

:   `Mandant, Operator`

    

**`FK_TRANSPORTLINES_OUTROUTES`**

:   `Mandant, OutboundRoute`

    

**`PK_TRANSPORTLINES`**

:   `Mandant, ID`

    
