# Tabelle **tblStudentComplexReports**



## Spalten

Diese Tabelle hat 10 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`PrevID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`EnbreaID`**

:   [`VARCHAR(24)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`StudentAchievement`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`Profile`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`Group`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`Entry`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`Grade`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`Report`**

:   [`BLOB subtype text  `](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

    

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`PK_COMPLEXREPORTS`**

:   `Mandant, ID`

    

## Fremdschlüssel

Diese Tabelle hat 3 Fremdschlüssel.

**`FK_COMPLEXREPORTS_GRADE`**

:   `Grade, Mandant` » [`GradeEntries (ID, Mandant)`](../../tables/gradeentries) · `ON UPDATE CASCADE` · `ON DELETE CASCADE`

    

**`FK_COMPLEXREPORTS_GROUP`**

:   `Group, Mandant` » [`AssessmentGroups (ID, Mandant)`](../../tables/assessmentgroups) · `ON UPDATE CASCADE` · `ON DELETE CASCADE`

    

**`FK_COMPLEXREPORTS_PROFILE`**

:   `Mandant, Profile` » [`AssessmentProfiles (ID, Mandant)`](../../tables/assessmentprofiles) · `ON UPDATE CASCADE` · `ON DELETE CASCADE`

    

## Indizes

Diese Ansicht hat 5 Indizes.

**`FK_COMPLEXREPORTS_ENTRY`**

:   `Mandant, Entry`

    

**`FK_COMPLEXREPORTS_GRADE`**

:   `Mandant, Grade`

    

**`FK_COMPLEXREPORTS_GROUP`**

:   `Mandant, Group`

    

**`FK_COMPLEXREPORTS_PROFILE`**

:   `Mandant, Profile`

    

**`PK_COMPLEXREPORTS`**

:   `Mandant, ID`

    
