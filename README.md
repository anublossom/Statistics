# Statistics → Correlation → Regression


## 1) Problem Statement (Exact Example)

I go to a shop every day and buy a bun.

Nominal values:

* Price = ₹5
* Weight = 10 grams

Because the shopkeeper is my friend, the **price varies**:

```
4.6, 4.7, 4.8, 4.9, 4.55, 4.66, 4.76, 4.88, 5.2, 5.3
```

The **bun weight also varies**:

```
9.98, 9.5, 9.6, 9.7, 9.8, 9.98, 10.3, 10.22, 10.13, 10.34
```

---

## 2) Variables and Paired Data

* x = price (₹)
* y = weight (grams)

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

Number of observations: n = 10

---

## 3) Mean (Average)

Mean formula:

```
mean = (sum of values) / n
```

Mean of x:

```
mean_x = 48.35 / 10 = 4.835
```

Mean of y:

```
mean_y = 99.55 / 10 = 9.955
```

---

## 4) Standard Deviation (All Steps)

### Step 1: Deviation from Mean and Squaring

| x    | x-mean_x | (x-mean_x)^2 | y     | y-mean_y | (y-mean_y)^2 |
| ---- | -------- | ------------ | ----- | -------- | ------------ |
| 4.60 | -0.235   | 0.055        | 9.98  | 0.025    | 0.001        |
| 4.70 | -0.135   | 0.018        | 9.50  | -0.455   | 0.207        |
| 4.80 | -0.035   | 0.001        | 9.60  | -0.355   | 0.126        |
| 4.90 | 0.065    | 0.004        | 9.70  | -0.255   | 0.065        |
| 4.55 | -0.285   | 0.081        | 9.80  | -0.155   | 0.024        |
| 4.66 | -0.175   | 0.031        | 9.98  | 0.025    | 0.001        |
| 4.76 | -0.075   | 0.006        | 10.30 | 0.345    | 0.119        |
| 4.88 | 0.045    | 0.002        | 10.22 | 0.265    | 0.070        |
| 5.20 | 0.365    | 0.133        | 10.13 | 0.175    | 0.031        |
| 5.30 | 0.465    | 0.216        | 10.34 | 0.385    | 0.148        |

---

### Step 2: Variance

Sample variance formula:

```
variance = sum((value - mean)^2) / (n - 1)
```

Variance of x:

```
variance_x = 0.547 / 9 = 0.061
```

Variance of y:

```
variance_y = 0.792 / 9 = 0.088
```

---

### Step 3: Standard Deviation

```
SD = sqrt(variance)
```

```
SD_x = sqrt(0.061) ≈ 0.25
SD_y = sqrt(0.088) ≈ 0.30
```

Interpretation:

* Typical price variation ≈ ±₹0.25
* Typical weight variation ≈ ±0.30 g

---

## 5) Correlation (r) — Full Calculation

Correlation formula (plain text):

```
r = sum[(x-mean_x)(y-mean_y)] / sqrt( sum(x-mean_x)^2 * sum(y-mean_y)^2 )
```

Compute numerator:

```
sum[(x-mean_x)(y-mean_y)] = 0.43
```

Compute denominator:

```
sqrt(0.547 * 0.792) = 0.658
```

Correlation:

```
r = 0.43 / 0.658 ≈ 0.49
```

Interpretation:

* r > 0 → positive relationship
* r ≈ 0.5 → moderate strength

---

## 6) Regression (y = a + b x)

Slope formula:

```
b = sum[(x-mean_x)(y-mean_y)] / sum(x-mean_x)^2
```

```
b = 0.43 / 0.547 ≈ 0.58
```

Intercept formula:

```
a = mean_y - b * mean_x
```

```
a = 9.955 - (0.58 * 4.835) ≈ 7.13
```

Regression equation:

```
y = 7.13 + 0.58 x
```

---

## 7) Probability of Deviation (z-score)

z-score formula:

```
z = (value - mean) / SD
```

Example: price = 5.30

```
z_x = (5.30 - 4.835) / 0.25 ≈ 1.86
```

Example: weight = 10.34

```
z_y = (10.34 - 9.955) / 0.30 ≈ 1.28
```

Values within ±2 SD are considered normal variation.

---

## 8) p-value (Significance of Correlation)

Test statistic:

```
t = r * sqrt(n - 2) / sqrt(1 - r^2)
```

```
t = 0.49 * sqrt(8) / sqrt(1 - 0.49^2) ≈ 1.56
```

Degrees of freedom:

```
df = n - 2 = 8
```

From t-table:

```
p ≈ 0.15
```

Interpretation:

* Trend exists
* Not statistically significant with small sample size

---

## Final Meaning

* Mean → typical value
* SD → normal variation
* Correlation → relationship strength
* Regression → predictive model
* p-value → reliability of the pattern

