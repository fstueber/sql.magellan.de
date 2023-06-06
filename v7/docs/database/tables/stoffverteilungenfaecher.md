# Tabelle **StoffverteilungenFaecher**



## Spalten

Diese Tabelle hat 3 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`Stoffverteilung`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`Fach`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`PK_STOFFFAECHER`**

:   `Mandant, Stoffverteilung, Fach`

    

## Fremdschlüssel

Diese Tabelle hat einen Fremdschlüssel.

**`FK_STOFFFACH_STOFF`**

:   `Mandant, Stoffverteilung` » [`Stoffverteilungen (ID, Mandant)`](../../tables/stoffverteilungen) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

    

## Indizes

Diese Ansicht hat 3 Indizes.

**`FK_STOFFFACH_FACH`**

:   `Mandant, Fach`

    

**`FK_STOFFFACH_STOFF`**

:   `Mandant, Stoffverteilung`

    

**`PK_STOFFFAECHER`**

:   `Mandant, Stoffverteilung, Fach`

    
