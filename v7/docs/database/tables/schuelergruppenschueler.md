# Tabelle **SchuelergruppenSchueler**



## Spalten

Diese Tabelle hat 5 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`Schueler`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`Schuelergruppe`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`Zugang`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes)

    

**`Abgang`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes)

    

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`PK_SGRUPPENSCHUELER`**

:   `Mandant, Schueler, Schuelergruppe`

    

## Fremdschlüssel

Diese Tabelle hat einen Fremdschlüssel.

**`FK_SGRUPPENSCHUELER_SCHUELER`**

:   `Mandant, Schueler` » [`Schueler (ID, Mandant)`](../../tables/schueler) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

    

## Indizes

Diese Ansicht hat 3 Indizes.

**`FK_SGRUPPENSCHUELER_GRUPPE`**

:   `Mandant, Schuelergruppe`

    

**`FK_SGRUPPENSCHUELER_SCHUELER`**

:   `Mandant, Schueler`

    

**`PK_SGRUPPENSCHUELER`**

:   `Mandant, Schueler, Schuelergruppe`

    
