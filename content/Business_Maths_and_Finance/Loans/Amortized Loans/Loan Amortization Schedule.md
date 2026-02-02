---
draft: false
---
This is a schedule of an [[Amortized Loans|amortized loan]], 

| Year | Principal at $nth$ year | [[Annuity]] Payment | Interest Portion | Principal Portion | Outstanding Balance Remaining |
| ---- | ----------------------- | ------------------- | ---------------- | ----------------- | ----------------------------- |
| 1    | $9,000                  | $2,878              | $1,620           | $1,258.00         | $7,742.00                     |
| 2    | $7,742                  | $2,878              | $1,398.56        | $1,484.44         | $6,257.56                     |
| 3    | $6,257.56               | $2,878              | $1,126.36        | $1,751.64         | $4,505.92                     |
| 4    | $4,505.92               | $2,878              | $811.07          | $2,066.93         | $2,458.98                     |
| 5    | $2,458.98               | $2,878              | $439.02          | $2,438.98         | $0.00                         |

# Steps
1. Get the nth year's starting principal.
2. Product of Annuity payment by the Interest Rate for Interest Portion.
3. Difference of Annuity Payment and Interest Portion for Principal Portion.
4. Difference of Principal at nth year and Principal Portion for next $(n+1)th$ year.

The annuity payment is always the same in an amortized loan, but the ratio of **interest** and **principal** payment always differ per year. 
