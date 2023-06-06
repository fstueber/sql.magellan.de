# Tabelle **StudentTransportation**



## Spalten

Diese Tabelle hat 6 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`EnbreaID`**

:   [`VARCHAR(24)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Student`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`InboundRoute`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`OutboundRoute`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`PK_STUDENTTRANSPORT`**

:   `Mandant, ID`

    

## Fremdschlüssel

Diese Tabelle hat 2 Fremdschlüssel.

**`FK_STUDENTTRANSPORT_OUTROUTES`**

:   `Mandant, OutboundRoute` » [`StudentRoutes (ID, Mandant)`](../../tables/studentroutes) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

    

**`FK_STUDENTTRANSPORT_SCHUELER`**

:   `Mandant, Student` » [`Schueler (ID, Mandant)`](../../tables/schueler) · `ON UPDATE CASCADE` · `ON DELETE CASCADE`

    

## Indizes

Diese Ansicht hat 4 Indizes.

**`FK_STUDENTTRANSPORT_INROUTES`**

:   `Mandant, InboundRoute`

    

**`FK_STUDENTTRANSPORT_OUTROUTES`**

:   `Mandant, OutboundRoute`

    

**`FK_STUDENTTRANSPORT_SCHUELER`**

:   `Mandant, Student`

    

**`PK_STUDENTTRANSPORT`**

:   `Mandant, ID`

    
