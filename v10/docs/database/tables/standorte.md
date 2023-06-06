# Tabelle **Standorte**



## Spalten

Diese Tabelle hat 4 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`Kuerzel`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    

**`Bezeichnung`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Gebaeude`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`PK_STANDORTE`**

:   `Mandant, Kuerzel`

    

## Fremdschlüssel

Diese Tabelle hat einen Fremdschlüssel.

**`FK_STANDORT_MANDANT`**

:   `Mandant` » [`Mandanten (ID)`](../../tables/mandanten) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

    

## Indizes

Diese Ansicht hat 3 Indizes.

**`FK_STANDORT_GEBAEUDE`**

:   `Mandant, Gebaeude`

    

**`FK_STANDORT_MANDANT`**

:   `Mandant`

    

**`PK_STANDORTE`**

:   `Mandant, Kuerzel`

    
