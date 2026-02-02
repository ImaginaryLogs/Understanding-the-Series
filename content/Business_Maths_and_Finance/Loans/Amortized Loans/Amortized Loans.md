---
draft: false
---
These are loans paid of in equal payments, and each loan payment is considered an [[Annuity]].^amortized-loans-def

Examples include *home mortgage loans* and *auto loans*.

In an amortized loan, interest payment declines each year as the amount owed declines and more of the principal is repaid.

$$
\text{PV}=\text{PMT}
\left[
\dfrac{ 1-\dfrac{1}{(1+i_\text{annual rate})^{n_\text{years}}}}
{i_\text{annual rate}}
\right]
$$



# Amortized Loans with Monthly Payments
If a amortized loan has monthly payments, then the formula must be adjusted to for month calculation.

$$
\text{PV}=\text{PMT}
\left[
\dfrac{
	1-\dfrac{1}{(1+\dfrac{i_\text{annual rate}}{m})^{n_\text{years} \times m}}
}
{\dfrac{i_\text{annual rate}}{m}}
\right]
$$


