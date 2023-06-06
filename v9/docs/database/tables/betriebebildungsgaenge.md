# Tabelle **BetriebeBildungsgaenge**



## Spalten

Diese Tabelle hat 3 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`Betrieb`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`Bildungsgang`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`PK_BETRIEBEBILDUNGSGAENGE`**

:   `Mandant, Betrieb, Bildungsgang`

    

## Fremdschlüssel

Diese Tabelle hat einen Fremdschlüssel.

**`FK_BETRIEBEBG_BILDUNGSGANG`**

:   `Bildungsgang` » [`Bildungsgaenge (Kuerzel)`](../../tables/bildungsgaenge) · `ON UPDATE CASCADE` · `ON DELETE CASCADE`

    

## Indizes

Diese Ansicht hat 3 Indizes.

**`FK_BETRIEBEBG_BETRIEB`**

:   `Mandant, Betrieb`

    

**`FK_BETRIEBEBG_BILDUNGSGANG`**

:   `Bildungsgang`

    

**`PK_BETRIEBEBILDUNGSGAENGE`**

:   `Mandant, Betrieb, Bildungsgang`

    
