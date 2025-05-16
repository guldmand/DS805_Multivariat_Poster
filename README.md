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


## Forbedret plan med Chattens hjælp


## Posterplan – Path 1 (Inferens om middelvektor)

### 1. Exploratory Data Analysis (EDA)
- Boxplots af længde og vægt efter køn
- Scatterplot (længde vs. vægt), farvet efter køn
- Normalitet: QQ-plots, tæthedskurver
- Multivariat normalitetstest (Mardia eller Shapiro)

### 2. Univariate test (supplerende)
- T-test for længde ~ køn
- T-test for vægt ~ køn

### 3. Multivariat test
- **Hotelling’s T² test**
  - H₀: μ_female = μ_male
  - Test af forskel i middelvektorer

### 4. Test for kovariansmatricer
- Box’s M test: Er det rimeligt at antage fælles kovariansmatrix?

### 5. Simultane konfidensintervaller (Bonferroni)
- 95% CI’er for forskellen i gennemsnit på længde og vægt

### 6. Konklusion og fortolkning
- Statistisk og biologisk betydning
