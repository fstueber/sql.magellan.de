# Tabelle **KlassenZeitraeume**



## Spalten

Diese Tabelle hat 20 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`EnbreaID`**

:   [`VARCHAR(24)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Klasse`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`Zeitraum`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`GUIDExtern`**

:   [`VARCHAR(40)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Jahrgang`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`Klassenleiter1`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`Klassenleiter2`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`Klassenstufe`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Fachtafel`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Unterrichtsform`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Unterrichtstage`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`Klassensprecher1`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`Klassensprecher2`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`Klassenelternsprecher1`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`Klassenelternsprecher2`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`Klassenwahlvertreter1`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`Klassenwahlvertreter2`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`Klassenraum`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`PK_KLASSENZEITRAEUME`**

:   `Mandant, Klasse, Zeitraum`

    

## Fremdschlüssel

Diese Tabelle hat 13 Fremdschlüssel.

**`FK_KLASSENZEITRAEUME_ELTERN2`**

:   `Klassenelternsprecher2, Mandant` » [`Sorgeberechtigte (ID, Mandant)`](../../tables/sorgeberechtigte) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

    

**`FK_KLASSENZEITRAEUME_FACHTAFEL`**

:   `Fachtafel, Mandant` » [`Fachtafeln (Kuerzel, Mandant)`](../../tables/fachtafeln) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

    

**`FK_KLASSENZEITRAEUME_KLASSE`**

:   `Klasse, Mandant` » [`Klassen (ID, Mandant)`](../../tables/klassen) · `ON UPDATE CASCADE` · `ON DELETE CASCADE`

    

**`FK_KLASSENZEITRAEUME_LEITER1`**

:   `Klassenleiter1, Mandant` » [`tblLehrer (ID, Mandant)`](../../tables/tbllehrer) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

    

**`FK_KLASSENZEITRAEUME_LEITER2`**

:   `Klassenleiter2, Mandant` » [`tblLehrer (ID, Mandant)`](../../tables/tbllehrer) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

    

**`FK_KLASSENZEITRAEUME_RAUM`**

:   `Klassenraum, Mandant` » [`Raeume (ID, Mandant)`](../../tables/raeume) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

    

**`FK_KLASSENZEITRAEUME_SPRECHER1`**

:   `Klassensprecher1, Mandant` » [`Schueler (ID, Mandant)`](../../tables/schueler) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

    

**`FK_KLASSENZEITRAEUME_SPRECHER2`**

:   `Klassensprecher2, Mandant` » [`Schueler (ID, Mandant)`](../../tables/schueler) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

    

**`FK_KLASSENZEITRAEUME_STUFE`**

:   `Klassenstufe` » [`Klassenstufen (Kuerzel)`](../../tables/klassenstufen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

    

**`FK_KLASSENZEITRAEUME_UNTERRICHT`**

:   `Unterrichtsform` » [`Unterrichtsformen (Kuerzel)`](../../tables/unterrichtsformen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

    

**`FK_KLASSENZEITRAEUME_WAHL1`**

:   `Klassenwahlvertreter1, Mandant` » [`Sorgeberechtigte (ID, Mandant)`](../../tables/sorgeberechtigte) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

    

**`FK_KLASSENZEITRAEUME_WAHL2`**

:   `Klassenwahlvertreter2, Mandant` » [`Sorgeberechtigte (ID, Mandant)`](../../tables/sorgeberechtigte) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

    

**`FK_KLASSENZEITRAEUME_ZEITRAUM`**

:   `Zeitraum` » [`Zeitraeume (ID)`](../../tables/zeitraeume) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

    

## Indizes

Diese Ansicht hat 16 Indizes.

**`FK_KLASSENZEITRAEUME_ELTERN1`**

:   `Mandant, Klassenelternsprecher1`

    

**`FK_KLASSENZEITRAEUME_ELTERN2`**

:   `Mandant, Klassenelternsprecher2`

    

**`FK_KLASSENZEITRAEUME_FACHTAFEL`**

:   `Mandant, Fachtafel`

    

**`FK_KLASSENZEITRAEUME_KLASSE`**

:   `Mandant, Klasse`

    

**`FK_KLASSENZEITRAEUME_LEITER1`**

:   `Mandant, Klassenleiter1`

    

**`FK_KLASSENZEITRAEUME_LEITER2`**

:   `Mandant, Klassenleiter2`

    

**`FK_KLASSENZEITRAEUME_RAUM`**

:   `Mandant, Klassenraum`

    

**`FK_KLASSENZEITRAEUME_SPRECHER1`**

:   `Mandant, Klassensprecher1`

    

**`FK_KLASSENZEITRAEUME_SPRECHER2`**

:   `Mandant, Klassensprecher2`

    

**`FK_KLASSENZEITRAEUME_STUFE`**

:   `Klassenstufe`

    

**`FK_KLASSENZEITRAEUME_UNTERRICHT`**

:   `Unterrichtsform`

    

**`FK_KLASSENZEITRAEUME_WAHL1`**

:   `Mandant, Klassenwahlvertreter1`

    

**`FK_KLASSENZEITRAEUME_WAHL2`**

:   `Mandant, Klassenwahlvertreter2`

    

**`FK_KLASSENZEITRAEUME_ZEITRAUM`**

:   `Zeitraum`

    

**`PK2_KLASSENZEITRAEUME`**

:   `Mandant, ID`

    

**`PK_KLASSENZEITRAEUME`**

:   `Mandant, Klasse, Zeitraum`

    
