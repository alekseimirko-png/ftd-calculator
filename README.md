# FTD Calculator

**A free calculator that turns an advertising budget into projected first-time deposits — and shows where the money stops being money.**

Live tool: **https://anaxeo.com/ftd-calculator**
No signup, no email capture, nothing stored. It runs entirely in the browser.

---

## Why this exists

Most paid campaigns in deposit-based industries are bought, optimised and reported on leads. Cost per lead falls month after month, the dashboard looks healthier every week, and the deposit count sits still.

A lead is a contact record. It becomes revenue only when somebody funds an account.

This calculator makes that gap visible. You enter your own figures, and it walks the money down the funnel one stage at a time until only the deposits are left.

---

## The model

Six inputs, in the order the funnel actually runs:

| Input | What it means |
|---|---|
| Monthly ad spend | Media budget for the month, excluding fees |
| CPM | Cost per thousand impressions in your market |
| Click-through rate | Share of impressions that become clicks |
| Page to registration | Share of visitors who complete a registration |
| Registration to deposit | Share of registrations that fund an account |
| Average first deposit | Typical size of a first deposit |
| Deposits per customer | Total deposits including the first, across the lifetime |

### The arithmetic

```
impressions   = (spend / CPM) × 1000
clicks        = impressions × CTR
registrations = clicks × page_conversion_rate
deposits      = registrations × registration_to_deposit_rate

cost per deposit = spend / deposits
first revenue    = deposits × average_first_deposit
lifetime revenue = deposits × average_first_deposit × deposits_per_customer
ROAS             = lifetime_revenue / spend
deposits per week = deposits / 4.33
```

Every stage multiplies. That is the whole point: a small change early in the chain produces a large change at the end, and a change at the end changes nothing upstream.

---

## What the output tells you

**Cost per deposit** rather than cost per lead. The only cost attached to money arriving.

**Return on ad spend** across the customer lifetime, not the first payment alone.

**Deposits per week.** Advertising delivery systems need a reasonable volume of conversion events to stabilise. Where deposits are too rare to reach that volume, campaigns stay in a learning state and costs swing regardless of targeting quality.

**Which lever moves it most.** A ten percent improvement applied to each input in turn, ranked by effect on margin. Mathematically the rate inputs all multiply equally — what differs is how achievable each improvement actually is.

---

## No benchmarks

The tool ships with no industry averages and no suggested figures beyond neutral defaults, deliberately.

Conversion rates differ by vertical, market, traffic source and offer. Any number published as a benchmark is a figure taken from somebody else's account and sold to you as yours.

Put your own numbers in — or the numbers somebody has promised you, and see whether the arithmetic survives.

---

## Related tool

**Ad Account Downtime Calculator** — https://anaxeo.com/downtime-calculator

In restricted and regulated categories advertising accounts stop working. That calculator prices a year of interruptions: unspent budget during dark days, revenue not produced while delivery relearns after each restart, and team hours spent rebuilding rather than buying.

---

## Reference

A glossary of the terminology used in both tools — FTD, qualified lead, learning phase, pre-lander, quality score, server-side tracking and forty-two others — is at **https://anaxeo.com/glossary**

---

## Notes

Built by [Anaxeo](https://anaxeo.com), a performance marketing team working across restricted, regulated and white niche categories.

This is arithmetic, not a forecast. It cannot tell you what your conversion rates will be — only what has to be true for a plan to work. If the required numbers look implausible, that is the finding.

---

## Licence

The calculator is free to use. Link back if it was useful to you.
