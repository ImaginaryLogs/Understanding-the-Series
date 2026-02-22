---
draft: false
---

Used to answer the generally question: 
> "*How much did my actual bank account grow? What was the compound annual growth rate (CAGR)?*"

It is given by the equation:
$$
G_{mean} = [((1+r_1)\cdot(1+r_2)\cdot\cdots)^{\frac{1}{n}}-1] = [(\prod_{i=1}^{n}{1+r_i})^{\frac{1}{n}}-1]
$$



# Real world application
Imagine you have ₱1,000,000 to invest. You are choosing between Investment A (a volatile Tech Stock) and Investment B (a stable Index Fund).

| **Year**   | **Investment A (Tech Stock)** | **Investment B (Index Fund)** |
| ---------- | ----------------------------- | ----------------------------- |
| **Year 1** | +40%                          | +10%                          |
| **Year 2** | -30%                          | +10%                          |
| **Year 3** | +50%                          | +10%                          |
Then, the growth rate of an investment is given by the geometric average. 
- **Investment A:** $[(1.40 \times 0.70 \times 1.50)^{1/3} - 1] \approx \mathbf{13.7\%}$
- **Investment B:** $[(1.10 \times 1.10 \times 1.10)^{1/3} - 1] = \mathbf{10\%}$

As a financial manager, you we see that wealth actually grew by 13.7% for investment A. The [[Arithmetic Average]] would return 20%; the gap exist because of the volatility (30%) ate the gains - this is the [[Risk]] present in the investment. 

