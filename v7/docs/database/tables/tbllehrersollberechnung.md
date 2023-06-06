# Tabelle **tblLehrerSollBerechnung**



## Spalten

Diese Tabelle hat 8 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`Lehrer`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`Von`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes)

    

**`Bis`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes)

    

**`Position`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`Dauer`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

    

**`LehrerSollSchluessel`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`PK_LEHRERSOLLBERECHNUNG`**

:   `Mandant, ID`

    

## Fremdschlüssel

Diese Tabelle hat einen Fremdschlüssel.

**`FK_LEHRERSOLLBERECHNUNG_MANDANT`**

:   `Mandant` » [`Mandanten (ID)`](../../tables/mandanten) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

    

## Indizes

Diese Ansicht hat 3 Indizes.

**`FK_LEHRERSOLLBERECHNUNG_LEHRER`**

:   `Mandant, Lehrer`

    

**`FK_LEHRERSOLLBERECHNUNG_MANDANT`**

:   `Mandant`

    

**`PK_LEHRERSOLLBERECHNUNG`**

:   `Mandant, ID`

    
