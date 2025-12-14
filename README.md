# Statistics → Correlation → Regression


## 1️⃣ Problem Statement (Exact Example)

 I go to a shop every day and buy a bun.

 Nominal values:

* Price = ₹5
* Weight = 10 grams

 Because the shopkeeper is my friend, the **price varies**:

`4.6, 4.7, 4.8, 4.9, 4.55, 4.66, 4.76, 4.88, 5.2, 5.3`

The **bun weight also varies**:

`9.98, 9.5, 9.6, 9.7, 9.8, 9.98, 10.3, 10.22, 10.13, 10.34`

---

## 2️⃣ Define Variables and Paired Data

Let:

* **x = price (₹)**
* **y = weight (grams)**

| Day | x    | y     |
| --- | ---- | ----- |
| 1   | 4.60 | 9.98  |
| 2   | 4.70 | 9.50  |
| 3   | 4.80 | 9.60  |
| 4   | 4.90 | 9.70  |
| 5   | 4.55 | 9.80  |
| 6   | 4.66 | 9.98  |
| 7   | 4.76 | 10.30 |
| 8   | 4.88 | 10.22 |
| 9   | 5.20 | 10.13 |
| 10  | 5.30 | 10.34 |

Number of observations: **n = 10**

---

## 3️⃣ Mean (Average)

### Mean of x

[ \bar{x} = \frac{\sum x}{n} = \frac{48.35}{10} = 4.835 ]

### Mean of y

[ \bar{y} = \frac{\sum y}{n} = \frac{99.55}{10} = 9.955 ]

---

## 4️⃣ Standard Deviation (Complete Calculation)

### 4.1 Deviation from Mean

| x    | x−x̄   | (x−x̄)² | y     | y−ȳ    | (y−ȳ)² |
| ---- | ------ | ------- | ----- | ------ | ------ |
| 4.60 | −0.235 | 0.055   | 9.98  | 0.025  | 0.001  |
| 4.70 | −0.135 | 0.018   | 9.50  | −0.455 | 0.207  |
| 4.80 | −0.035 | 0.001   | 9.60  | −0.355 | 0.126  |
| 4.90 | 0.065  | 0.004   | 9.70  | −0.255 | 0.065  |
| 4.55 | −0.285 | 0.081   | 9.80  | −0.155 | 0.024  |
| 4.66 | −0.175 | 0.031   | 9.98  | 0.025  | 0.001  |
| 4.76 | −0.075 | 0.006   | 10.30 | 0.345  | 0.119  |
| 4.88 | 0.045  | 0.002   | 10.22 | 0.265  | 0.070  |
| 5.20 | 0.365  | 0.133   | 10.13 | 0.175  | 0.031  |
| 5.30 | 0.465  | 0.216   | 10.34 | 0.385  | 0.148  |

---

### 4.2 Variance and SD

[ \text{Variance}_x = \frac{0.547}{9} = 0.061 ]
[ SD_x = \sqrt{0.061} \approx 0.25 ]

[ \text{Variance}_y = \frac{0.792}{9} = 0.088 ]
[ SD_y = \sqrt{0.088} \approx 0.30 ]

---

## 5️⃣ Correlation (Full Calculation)

### 5.1 Product of Deviations

[ (x_i-x̄)(y_i-ȳ) ]

Sum:
[ \sum (x_i-x̄)(y_i-ȳ) = 0.43 ]

---

### 5.2 Correlation Formula

[ r = \frac{\sum (x_i-x̄)(y_i-ȳ)}{\sqrt{\sum (x_i-x̄)^2 \sum (y_i-ȳ)^2}} ]

[ r = \frac{0.43}{\sqrt{0.547 \times 0.792}} \approx 0.49 ]

---

## 6️⃣ Regression (y = a + bx)

### 6.1 Slope

[ b = \frac{\sum (x_i-x̄)(y_i-ȳ)}{\sum (x_i-x̄)^2} = \frac{0.43}{0.547} \approx 0.58 ]

### 6.2 Intercept

[ a = ȳ - b x̄ = 9.955 - (0.58)(4.835) = 7.13 ]

### Regression Equation

[ \boxed{y = 7.13 + 0.58x} ]

---

## 7️⃣ Probability of Deviation (z‑score)

### Example: Paying ₹5.30

[ z_x = \frac{5.30 - 4.835}{0.25} = 1.86 ]

### Example: Weight 10.34 g

[ z_y = \frac{10.34 - 9.955}{0.30} = 1.28 ]

Interpretation:

* Values within ±2 SD are **normal variation**

---

## 8️⃣ p‑Value (Significance of Correlation)

[ t = \frac{r\sqrt{n-2}}{\sqrt{1-r^2}} ]

[ t = \frac{0.49\sqrt{8}}{\sqrt{1-0.49^2}} \approx 1.56 ]

Degrees of freedom:
[ df = 8 ]

From t‑distribution:
[ p \approx 0.15 ]

---


