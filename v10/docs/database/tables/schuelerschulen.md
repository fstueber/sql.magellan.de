# Tabelle **SchuelerSchulen**



## Spalten

Diese Tabelle hat 17 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`EnbreaID`**

:   [`VARCHAR(24)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Schueler`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`Schule`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`Schulform`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Schulart`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Von`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes)

    

**`Bis`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes)

    

**`LetzteKlasse`**

:   [`VARCHAR(15)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Klassenleiter`**

:   [`VARCHAR(50)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Abschluss`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Herkunft`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Unterlagen`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Sprachfoerderung`**

:   [`CHAR(1) `](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Laufbahn`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`Klassenstufe`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`PK_SCHUELERSCHULEN`**

:   `Mandant, ID`

    

## Fremdschlüssel

Diese Tabelle hat 6 Fremdschlüssel.

**`FK_SCHUELERS_SCHUELER`**

:   `Mandant, Schueler` » [`Schueler (ID, Mandant)`](../../tables/schueler) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

    

**`FK_SCHUELERS_SCHULART`**

:   `Schulart` » [`SchulartenHerkunft (Kuerzel)`](../../tables/schulartenherkunft) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

    

**`FK_SCHUELERS_SCHULE`**

:   `Schule` » [`Schulen (ID)`](../../tables/schulen) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

    

**`FK_SCHUELERS_SCHULFORM`**

:   `Schulform` » [`SchulformenHerkunft (Kuerzel)`](../../tables/schulformenherkunft) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

    

**`FK_SCHUELERS_STUFE`**

:   `Klassenstufe` » [`Klassenstufen (Kuerzel)`](../../tables/klassenstufen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

    

**`FK_SCHUELERS_UNTERLAGEN`**

:   `Unterlagen` » [`Herkunftsunterlagen (Kuerzel)`](../../tables/herkunftsunterlagen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

    

## Indizes

Diese Ansicht hat 8 Indizes.

**`FK_SCHUELERS_HERKUNFT`**

:   `Herkunft`

    

**`FK_SCHUELERS_SCHUELER`**

:   `Mandant, Schueler`

    

**`FK_SCHUELERS_SCHULART`**

:   `Schulart`

    

**`FK_SCHUELERS_SCHULE`**

:   `Schule`

    

**`FK_SCHUELERS_SCHULFORM`**

:   `Schulform`

    

**`FK_SCHUELERS_STUFE`**

:   `Klassenstufe`

    

**`FK_SCHUELERS_UNTERLAGEN`**

:   `Unterlagen`

    

**`PK_SCHUELERSCHULEN`**

:   `Mandant, ID`

    
