---
draft: false
---

- The anticipated return from an investment accounted in all possibilities, 
- Expressed in **percentage**. 
- Probability-weight average of all potential outcomes.

$$
E[R]=\sum_{i=1}^n{\text{Return}_i\cdot\text{Probability}_i}
$$
Used best for **asset allocation**, used best to see if the total portfolio meets your target.



Relies on [[Historical Evidence]] and Probability Estimates. They rely on the [[historical frequency method]] or [[scenario analysis method]].

For an investment like in stocks, the range of price of an investment is represented by a normal distribution.

Expected return is the center of that bell curve, the mu.

![[Pasted image 20260223031543.png]]

# Instance

**Given**: Imagine you have ₱1,000,000 to invest. You are choosing between Investment A (a volatile Tech Stock) and Investment B (a stable Index Fund).

| Year       | Investment A (Tech Stock) | Investment B (Index Fund) |
| ---------- | ------------------------- | ------------------------- |
| Year 1 | +40%                      | +10%                      |
| Year 2 | -30%                      | +10%                      |
| Year 3 | +50%                      | +10%                      |

**Task**: Suppose you decide to build a **Portfolio** with 50% in A and 50% in B. 

**Assumption**: You expect the economy has a 70% chance of being "Good" (A does 20%, B does 10%), and a 30% chance of being "Bad" (A does -10%, B does 5%). 

Calculate Expected Return for A: $(0.70 \times 20) + (0.30 \times -10) = 11\%$

Calculate Expected Return for B: $(0.70 \times 10) + (0.30 \times 5) = 8.5\%$

Portfolio $E(R)$: $(0.50 \times 11\%) + (0.50 \times 8.5\%) = \mathbf{9.75\%}$

Adjusting the weight of which assets to invest can lead to a different values of expected return.