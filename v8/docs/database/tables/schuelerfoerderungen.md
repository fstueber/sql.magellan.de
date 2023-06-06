# Tabelle **SchuelerFoerderungen**



## Spalten

Diese Tabelle hat 16 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`EnbreaID`**

:   [`VARCHAR(24)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Schueler`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`Behinderung`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Beeintraechtigung`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Schwerpunkt1`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Schwerpunkt2`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Bedarf`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Ausgleich`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Gefoerdert`**

:   [`CHAR(1) `](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Stunden1`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

    

**`Stunden2`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

    

**`Position`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`Von`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes)

    

**`Bis`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes)

    

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`PK_SCHUELERFOERDERUNGEN`**

:   `Mandant, ID`

    

## Fremdschlüssel

Diese Tabelle hat 5 Fremdschlüssel.

**`FK_SCHUELERFOERDER_BEDARF`**

:   `Bedarf` » [`SopaedFoerderungen (Kuerzel)`](../../tables/sopaedfoerderungen) · `ON UPDATE NO ACTION` · `ON DELETE SET NULL`

    

**`FK_SCHUELERFOERDER_BEHINDERUNG`**

:   `Behinderung` » [`Behinderungsarten (Kuerzel)`](../../tables/behinderungsarten) · `ON UPDATE NO ACTION` · `ON DELETE SET NULL`

    

**`FK_SCHUELERFOERDER_SCHUELER`**

:   `Mandant, Schueler` » [`Schueler (ID, Mandant)`](../../tables/schueler) · `ON UPDATE NO ACTION` · `ON DELETE CASCADE`

    

**`FK_SCHUELERFOERDER_SCHWERPUNKT1`**

:   `Schwerpunkt1` » [`FoerderSchwerpunkte (Kuerzel)`](../../tables/foerderschwerpunkte) · `ON UPDATE NO ACTION` · `ON DELETE SET NULL`

    

**`FK_SCHUELERFOERDER_SCHWERPUNKT2`**

:   `Schwerpunkt2` » [`FoerderSchwerpunkte (Kuerzel)`](../../tables/foerderschwerpunkte) · `ON UPDATE NO ACTION` · `ON DELETE SET NULL`

    

## Indizes

Diese Ansicht hat 7 Indizes.

**`FK_SCHUELERFOERDER_AUSGLEICH`**

:   `Ausgleich`

    

**`FK_SCHUELERFOERDER_BEDARF`**

:   `Bedarf`

    

**`FK_SCHUELERFOERDER_BEHINDERUNG`**

:   `Behinderung`

    

**`FK_SCHUELERFOERDER_SCHUELER`**

:   `Mandant, Schueler`

    

**`FK_SCHUELERFOERDER_SCHWERPUNKT1`**

:   `Schwerpunkt1`

    

**`FK_SCHUELERFOERDER_SCHWERPUNKT2`**

:   `Schwerpunkt2`

    

**`PK_SCHUELERFOERDERUNGEN`**

:   `Mandant, ID`

    
