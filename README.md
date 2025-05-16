# DS805_Multivariat_Poster
Multivariat Statistisk Analyse Poster Project



## Plan

**EDA**
- normalfordeling
- tæthedskurve

**Univariate**
- almindelige hypoteser vægt <-> køn        p1
- almindelige hypoteser længde <-> køn      p2

**Multivariat**
- H0 p1 middelværdi - p2 middelværdi = 0
- HA p1 middelværdi - p2 middelværdi != 0

- **Fordeling**

- **Annova**
- **Mannova**

- **Konklusioner**





<hr>


## Forbedret plan


## Posterplan – Path 1 (Inferens om middelvektor)

### 1. Exploratory Data Analysis (EDA)
- Boxplots af længde og vægt efter køn
- Scatterplot (længde vs. vægt), farvet efter køn
- Normalitet: QQ-plots, tæthedskurver
- Multivariat normalitetstest (Mardia eller Shapiro)

### 2. Univariate test (supplerende)
- T-test for længde ~ køn
- T-test for vægt ~ køn
- T

#Test af normalitets. 5.4b
qqplot for hver enkelt (univariat eller magninal normalitet)
Manalanobis multivariate (Multivariat normalitet)

### 3 konfidensintervallerne (5.4B, qqplot for hver, manhalobis af D2)

### 3. Mulitvariat normalitets test
- Se billedet

### 3. Multivariat test
- **Hotelling’s T² test**
  - H₀: μ_female = μ_male
  - Test af forskel i middelvektorer

### 4. Test for kovariansmatricer
- Box’s M test: Er det rimeligt at antage fælles kovariansmatrix?
- Opgave 6.19D

### 5. Simultane konfidensintervaller (Bonferroni, simultankonfidensinterval (T2))
- 95% CI’er for forskellen i gennemsnit på længde og vægt
Mulivariat forksel, Tjek om CI for snut og vægt, hvilken en af dem eller i begge er 0,0 inkluderet

Test 2 kovariansmatricer
Test om de er normalfordelte QQPLOT
+ Vi antager uafhængige og tilfældige stikprøver


### 6. Konklusion og fortolkning
- Statistisk og biologisk betydning






## Final poster

Tak! Du har nu udarbejdet en **rigtig stærk og præcis posterplan**, som er fagligt velfunderet og også stemmer overens med både:

* 📘 Kapitel 5 & 6 i *Applied Multivariate Statistical Analysis*
* 🧪 Opgave 6.39 i bogen
* ✅ Posterkravene til Path 1 (inferens)

Din undervisers feedback og dine noter (inkl. billeder) viser, at du **forstår hvordan univariat og multivariat inferens hænger sammen**, og hvordan du skal opbygge en stringent analyse og fortælling på posteren.

---

## 📌 Endelig og struktureret version af din plan

Her er din forbedrede plan, struktureret og formuleret som sektioner til din poster:

---

### 🟩 1. Exploratory Data Analysis (EDA)

* **Boxplots** for længde og vægt fordelt på køn
* **Scatterplot** (snout-vent length vs. vægt) farvet efter køn
* **Univariat normalitetstest**:

  * QQ-plot for længde og vægt i hver gruppe
  * Tæthedskurve sammen med normalfordeling
* **Multivariat normalitetstest**:

  * Mahalanobis afstande + QQ-plot af $D^2$ værdier
  * Brug fx `mvnormtest::mshapiro.test()` (kræver få observationer)
  * Alternativt: visuelt med `car::qqPlot()` og Mahalanobis

---

### 🟩 2. Univariate analyser (valgfri, men god støtte)

* **T-test** for:

  * længde vs. køn
  * vægt vs. køn
* Bruges til at supplere konklusionen fra multivariat test

---

### 🟩 3. Multivariat inferens

* **Hotelling’s T² test** for forskel i middelvektor:

  * $H_0: \mu_{\text{female}} = \mu_{\text{male}}$
  * $H_A: \mu_{\text{female}} \ne \mu_{\text{male}}$
* Hvis signifikant → fortsæt med simultane CI’er

---

### 🟩 4. Test for lighed i kovariansmatricer

* **Box’s M test**

  * Er varians/kovariansstrukturen ens i begge grupper?
  * Hvis ja → poolet kovariansmatrix
  * Hvis nej → brug separate kovarianser eller QDA senere

---

### 🟩 5. Simultane konfidensintervaller

* Brug Bonferroni eller T²-metode til simultane CI’er
* Undersøg om **nul** er inkluderet i CI for:

  * længde
  * vægt
* Fortolk: Hvilken af de to variable adskiller grupperne?

---

### 🟩 6. Antagelser og modelgrundlag

* Antag uafhængige og tilfældigt udvalgte observationer
* Vis evt. residualer fra t-testen (som i dit billede)
* Angiv om normalitetsantagelserne ser rimelige ud

---

### 🟩 7. Konklusion og fortolkning

* Statistisk betydning: Er forskellen signifikant?
* Biologisk betydning: Er forskellen stor/relevant i praksis?
* Er forskellen drevet af længde, vægt – eller begge?

---

## 💡 Klar til Rmd?

Hvis du er enig i denne plan, så kan jeg nu:

1. **Generere hele `.Rmd`-filen** med kode og plots
2. Organisere sektionerne som ovenfor (klar til poster)
3. Sikre, at output er klar til at blive kopieret ind i LaTeX, PowerPoint, Canva eller andet designværktøj

Skriv `lav .Rmd`, så starter vi.

