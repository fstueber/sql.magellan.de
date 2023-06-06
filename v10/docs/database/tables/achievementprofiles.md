# Tabelle **AchievementProfiles**



## Spalten

Diese Tabelle hat 14 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    

**`PrevID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`EnbreaID`**

:   [`VARCHAR(24)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Configuration`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`GradeSystem`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`GradeType`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`AssessmentProfile`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`ClassTerm`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`Course`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    

**`Code`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    

**`Name`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`Description`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

**`InternalCode`**

:   [`VARCHAR(3)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`PK_ACHIEVEMENTPROFILES`**

:   `Mandant, ID`

    

## Fremdschlüssel

Diese Tabelle hat 4 Fremdschlüssel.

**`FK_ACHIEVEPROFILE_CLASSTERM`**

:   `ClassTerm, Mandant` » [`KlassenZeitraeume (ID, Mandant)`](../../tables/klassenzeitraeume) · `ON UPDATE CASCADE` · `ON DELETE CASCADE`

    

**`FK_ACHIEVEPROFILE_COURSE`**

:   `Course, Mandant` » [`tblCourses (ID, Mandant)`](../../tables/tblcourses) · `ON UPDATE CASCADE` · `ON DELETE CASCADE`

    

**`FK_ACHIEVEPROFILE_GRADESYSTEM`**

:   `GradeSystem, Mandant` » [`GradeSystems (ID, Mandant)`](../../tables/gradesystems) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

    

**`FK_ACHIEVEPROFILE_GRADETYPE`**

:   `GradeType, Mandant` » [`GradeTypes (ID, Mandant)`](../../tables/gradetypes) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

    

## Indizes

Diese Ansicht hat 6 Indizes.

**`FK_ACHIEVEPROFILE_ASSMPROFILE`**

:   `Mandant, AssessmentProfile`

    

**`FK_ACHIEVEPROFILE_CLASSTERM`**

:   `Mandant, ClassTerm`

    

**`FK_ACHIEVEPROFILE_COURSE`**

:   `Mandant, Course`

    

**`FK_ACHIEVEPROFILE_GRADESYSTEM`**

:   `Mandant, GradeSystem`

    

**`FK_ACHIEVEPROFILE_GRADETYPE`**

:   `Mandant, GradeType`

    

**`PK_ACHIEVEMENTPROFILES`**

:   `Mandant, ID`

    
