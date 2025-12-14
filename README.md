# Statistics
**Imagine I go to a shop every day and buy a bun.**
The bun price is normally ₹5 and the bun weight is 10 grams.
Since the shopkeeper is my friend, sometimes I pay different prices like:
4.6, 4.7, 4.8, 4.9, 4.55, 4.66, 4.76, 4.88, 5.2, 5.3

Also, the bun weight is not always exactly 10 grams. It varies like:
9.98, 9.5, 9.6, 9.7, 9.8, 9.98, 10.3, 10.22, 10.13, 10.34
What all statistical quantities can we find from this data?

🔹 Step 1: Define Variables Clearly

We define:

x = price paid (₹)

y = bun weight (grams)

🔹 Step 2: Raw Data
x (Price in ₹)
4.6, 4.7, 4.8, 4.9, 4.55,
4.66, 4.76, 4.88, 5.2, 5.3


Number of observations = 10

y (Weight in grams)
9.98, 9.5, 9.6, 9.7, 9.8,
9.98, 10.3, 10.22, 10.13, 10.34


Number of observations = 10


🔹 Step 3: Mean (Average)
Mean of x (price)
𝑥
ˉ
=
4.6
+
4.7
+
4.8
+
4.9
+
4.55
+
4.66
+
4.76
+
4.88
+
5.2
+
5.3
10
x
ˉ
=
10
4.6+4.7+4.8+4.9+4.55+4.66+4.76+4.88+5.2+5.3
	​

𝑥
ˉ
=
48.35
10
=
4.835
x
ˉ
=
10
48.35
	​

=4.835

➡️ Average price paid = ₹4.835

Mean of y (weight)
𝑦
ˉ
=
9.98
+
9.5
+
9.6
+
9.7
+
9.8
+
9.98
+
10.3
+
10.22
+
10.13
+
10.34
10
y
ˉ
	​

=
10
9.98+9.5+9.6+9.7+9.8+9.98+10.3+10.22+10.13+10.34
	​

𝑦
ˉ
=
99.55
10
=
9.955
y
ˉ
	​

=
10
99.55
	​

=9.955

➡️ Average bun weight = 9.955 g



🔹 Step 4: Standard Deviation of x (Price) — STEP BY STEP
Purpose of SD

To measure how much the price normally deviates from the mean.

Step 4.1: Deviation from mean
𝑥
𝑖
−
𝑥
ˉ
x
i
	​

−
x
ˉ
x	
𝑥
−
𝑥
ˉ
x−
x
ˉ

4.60	−0.235
4.70	−0.135
4.80	−0.035
4.90	+0.065
4.55	−0.285
4.66	−0.175
4.76	−0.075
4.88	+0.045
5.20	+0.365
5.30	+0.465
Step 4.2: Square the deviations

(Removes sign and emphasizes larger errors)

Deviation	Square
−0.235	0.055
−0.135	0.018
−0.035	0.001
+0.065	0.004
−0.285	0.081
−0.175	0.031
−0.075	0.006
+0.045	0.002
+0.365	0.133
+0.465	0.216
Step 4.3: Variance of x
Variance
𝑥
=
∑
(
𝑥
𝑖
−
𝑥
ˉ
)
2
𝑛
−
1
Variance
x
	​

=
n−1
∑(x
i
	​

−
x
ˉ
)
2
	​

=
0.547
9
≈
0.061
=
9
0.547
	​

≈0.061
Step 4.4: Standard Deviation of x
SD
𝑥
=
0.061
≈
0.25
SD
x
	​

=
0.061
	​

≈0.25

➡️ Typical price variation = ±₹0.25

🔹 Step 5: Standard Deviation of y (Weight) — STEP BY STEP
Step 5.1: Deviation from mean
𝑦
𝑖
−
𝑦
ˉ
y
i
	​

−
y
ˉ
	​

y	
𝑦
−
𝑦
ˉ
y−
y
ˉ
	​


9.98	+0.025
9.50	−0.455
9.60	−0.355
9.70	−0.255
9.80	−0.155
9.98	+0.025
10.30	+0.345
10.22	+0.265
10.13	+0.175
10.34	+0.385
Step 5.2: Square the deviations
Deviation	Square
+0.025	0.001
−0.455	0.207
−0.355	0.126
−0.255	0.065
−0.155	0.024
+0.025	0.001
+0.345	0.119
+0.265	0.070
+0.175	0.031
+0.385	0.148
Step 5.3: Variance of y
Variance
𝑦
=
0.792
9
≈
0.088
Variance
y
	​

=
9
0.792
	​

≈0.088
Step 5.4: Standard Deviation of y
SD
𝑦
=
0.088
≈
0.30
SD
y
	​

=
0.088
	​

≈0.30

➡️ Typical weight variation = ±0.30 g
**📘 Part 2: Correlation and Regression**

🔹 Given Data (from Part 1)

We defined:

x = price paid (₹)

y = bun weight (grams)

Paired observations:

Day	x (Price ₹)	y (Weight g)
1	4.60	9.98
2	4.70	9.50
3	4.80	9.60
4	4.90	9.70
5	4.55	9.80
6	4.66	9.98
7	4.76	10.30
8	4.88	10.22
9	5.20	10.13
10	5.30	10.34

From Part 1:

Mean price, 
𝑥
ˉ
=
4.835
x
ˉ
=4.835

Mean weight, 
𝑦
ˉ
=
9.955
y
ˉ
	​

=9.955

🔹 What Question Are We Asking Now?

When the price paid changes, does the bun weight also change in a related way?

This question is answered by correlation.

1️⃣ CORRELATION
🔹 What Correlation Measures

Correlation measures:

How strongly and in what direction two variables move together

It does not:

Predict values

Explain cause

Give an equation

🔹 Step 1: Deviations from the Mean

We calculate deviations already used in Part 1:

(
𝑥
𝑖
−
𝑥
ˉ
)
,
(
𝑦
𝑖
−
𝑦
ˉ
)
(x
i
	​

−
x
ˉ
),(y
i
	​

−
y
ˉ
	​

)

Example (Day 1):

x deviation = 4.60 − 4.835 = −0.235
y deviation = 9.98 − 9.955 = +0.025

🔹 Step 2: Product of Deviations

For each day:

(
𝑥
𝑖
−
𝑥
ˉ
)
(
𝑦
𝑖
−
𝑦
ˉ
)
(x
i
	​

−
x
ˉ
)(y
i
	​

−
y
ˉ
	​

)

Why?

Same sign → variables move together

Opposite sign → variables move opposite

We sum all these products:

∑
(
𝑥
𝑖
−
𝑥
ˉ
)
(
𝑦
𝑖
−
𝑦
ˉ
)
≈
0.43
∑(x
i
	​

−
x
ˉ
)(y
i
	​

−
y
ˉ
	​

)≈0.43
🔹 Step 3: Normalize by Variations

Correlation coefficient:

𝑟
=
∑
(
𝑥
𝑖
−
𝑥
ˉ
)
(
𝑦
𝑖
−
𝑦
ˉ
)
∑
(
𝑥
𝑖
−
𝑥
ˉ
)
2
∑
(
𝑦
𝑖
−
𝑦
ˉ
)
2
r=
∑(x
i
	​

−
x
ˉ
)
2
∑(y
i
	​

−
y
ˉ
	​

)
2
	​

∑(x
i
	​

−
x
ˉ
)(y
i
	​

−
y
ˉ
	​

)
	​


Using values from Part 1:

𝑟
≈
0.49
r≈0.49
✅ Correlation Result
𝑟
≈
+
0.49
r≈+0.49
	​

Interpretation

Positive sign → higher price tends to come with higher weight

Magnitude ~0.5 → moderate relationship

Relationship exists, but not perfect

🔹 Meaning in This Example

When you pay more, the bun tends to weigh more,
but there is still significant variability.

2️⃣ REGRESSION
🔹 What Question Regression Answers

Correlation says:

“There is a relationship”

Regression asks:

“Can we write an equation to estimate weight from price?”

🔹 Regression Model

We assume a linear model:

𝑦
=
𝑎
+
𝑏
𝑥
y=a+bx

Where:

𝑦
y = bun weight

𝑥
x = price paid

𝑏
b = slope

𝑎
a = intercept

🔹 Step 1: Calculate Slope (b)
𝑏
=
∑
(
𝑥
𝑖
−
𝑥
ˉ
)
(
𝑦
𝑖
−
𝑦
ˉ
)
∑
(
𝑥
𝑖
−
𝑥
ˉ
)
2
b=
∑(x
i
	​

−
x
ˉ
)
2
∑(x
i
	​

−
x
ˉ
)(y
i
	​

−
y
ˉ
	​

)
	​


Using our values:

𝑏
≈
0.58
b≈0.58
🔹 Step 2: Calculate Intercept (a)
𝑎
=
𝑦
ˉ
−
𝑏
𝑥
ˉ
a=
y
ˉ
	​

−b
x
ˉ
𝑎
=
9.955
−
(
0.58
)
(
4.835
)
≈
7.13
a=9.955−(0.58)(4.835)≈7.13
✅ Regression Equation
𝑦
=
7.13
+
0.58
𝑥
y=7.13+0.58x
	​

🔹 Interpretation of the Equation

Slope (0.58)
→ For every extra ₹1 paid, expected bun weight increases by 0.58 g

Intercept (7.13)
→ Mathematical offset (not physically meaningful by itself)


🔹 Example Prediction

If you pay ₹5.0:

𝑦
=
7.13
+
0.58
(
5
)
=
10.03
 g
y=7.13+0.58(5)=10.03 g

So regression predicts:

Expected bun weight ≈ 10.03 g

Actual weight may vary around this.



📘 Part 3: Probability, Deviation, and p-Value

(Using the Same Shop Example)

🔹 What We Have So Far

From Part 1:

Mean price 
𝑥
ˉ
=
4.835
x
ˉ
=4.835

SD of price 
𝑆
𝐷
𝑥
≈
0.25
SD
x
	​

≈0.25

Mean weight 
𝑦
ˉ
=
9.955
y
ˉ
	​

=9.955

SD of weight 
𝑆
𝐷
𝑦
≈
0.30
SD
y
	​

≈0.30

From Part 2:

Correlation 
𝑟
≈
0.49
r≈0.49

Regression equation:

𝑦
=
7.13
+
0.58
𝑥
y=7.13+0.58x

Now we answer two new questions:

How unusual is a particular value?

Is the observed relationship real or could it be random?

1️⃣ PROBABILITY OF DEVIATION (z-SCORE)
🔹 What Is This Question?

If I pay a certain price or receive a certain weight,
how unusual is that value compared to normal behavior?

This is answered using standard deviation units.

🔹 z-Score Formula
𝑧
=
Observed value
−
Mean
Standard deviation
z=
Standard deviation
Observed value−Mean
	​


This converts a value into:

“How many SDs away from the mean?”

🔹 Example 1: Price Deviation

Suppose you paid ₹5.30.

𝑧
𝑥
=
5.30
−
4.835
0.25
≈
1.86
z
x
	​

=
0.25
5.30−4.835
	​

≈1.86
Interpretation

1.86 SD above the mean

Uncommon, but not extreme

Happens naturally sometimes

🔹 Example 2: Weight Deviation

Suppose bun weight is 10.34 g.

𝑧
𝑦
=
10.34
−
9.955
0.30
≈
1.28
z
y
	​

=
0.30
10.34−9.955
	​

≈1.28
Interpretation

About 1.3 SD above the mean

Very normal variation

🔹 What z-Score Tells Us
z-value	Meaning
0	Exactly average
±1	Very common
±2	Uncommon
±3	Rare

Your values are not outliers.

2️⃣ WHY PROBABILITY NEEDS A CURVE

When data is collected many times:

Most values cluster near the mean

Fewer values occur far away

This forms a bell-shaped curve.

The curve helps answer:

“How often should I expect a value this far from the mean?”

3️⃣ p-VALUE (STATISTICAL SIGNIFICANCE)
🔹 What Question Does p-Value Answer?

Is the observed price–weight relationship likely real,
or could it have happened by random chance?

🔹 Null Hypothesis (Starting Assumption)

Price and weight are unrelated

Statistics always starts by assuming no relationship.

🔹 What p-Value Measures

p-value answers:

If there was actually no relationship, how often would we see a correlation this strong just by chance?

🔹 Using Correlation to Compute p-Value

Test statistic:

𝑡
=
𝑟
𝑛
−
2
1
−
𝑟
2
t=
1−r
2
	​

r
n−2
	​

	​


Where:

𝑟
=
0.49
r=0.49

𝑛
=
10
n=10

𝑡
≈
1.56
t≈1.56

Degrees of freedom:

𝑑
𝑓
=
𝑛
−
2
=
8
df=n−2=8

From t-distribution:

𝑝
≈
0.15
p≈0.15
✅ p-Value Result
𝑝
≈
0.15
p≈0.15
	​

🔹 Interpretation of p-Value
p-value	Meaning
< 0.05	Strong evidence
0.05–0.1	Weak evidence
> 0.1	Not reliable

Here:

p = 0.15 → not statistically significant

🔹 What This Means in Simple Words

We see a trend where higher price tends to give higher weight,
but with this small and noisy dataset,
we cannot confidently say the relationship is real.

This does not mean:

The trend is false

The analysis is wrong

It means:

More data is needed

4️⃣ CONNECTING EVERYTHING TOGETHER
Tool	Question Answered
Mean	What is typical?
SD	How much variation is normal?
z-score	How unusual is a value?
Correlation	Do x and y move together?
Regression	Can we model y from x?
p-value	Can we trust the pattern?



