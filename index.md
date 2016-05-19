---
title       : Mortgage Calculator
subtitle    : www.scottdaviscre.info
author      : Scott Davis
job         : Mortgage Calculator
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Problem

With widespread recovery in the housing markets, people are actively re-entering the home purchase market.

Buyers need a good resource to evaluate the affordability of loans -- many mortgage calculators just show the mortgage payment.


---

## Proposed Solution

The full monthly cost of a mortgage is known as the "PITI" payment - principal and interest (mortgage), property taxes and property casualty insurance.

This is a quick calculator, accessible remotely, that prospective purchasers could use to quickly calculate their actual monthly mortgage cost.
---

## Submitted Solution

So to calculate the monthly mortgage cost for a home priced at $250,000 with a 6%, $50,000 down payment; 30-year fixed mortgage rate; $3.50 per $100 valuation tax rate; and an insurance premium of 2% of value:


```r
round((250000-50000)*(0.06/12)/(1-(1+(0.06/12))^(-(30*12))),2)
```

```
## [1] 1199.1
```

To calculate the tax payment portion:


```r
round((250000*(3.5/100))/12,2)
```

```
## [1] 729.17
```

and the insurance payment portion:


```r
round(((2/100)*250000)/12,2)
```

```
## [1] 416.67
```

So a prospective buyer could expect a monthly mortgage payment of 2344.94
 ---

## Thanks and feedback location

I hope this helps you with your property investing decisions.

Please direct feedback to scdavis50@gmail.com and visit www.scottdaviscre.info

Thanks you for your time and feedback.
