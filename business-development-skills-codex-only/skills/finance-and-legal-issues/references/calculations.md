# Financial calculation guide

Use Python or another reliable calculation tool. Keep EUR, selling unit, time period, VAT treatment, sources, and unknowns explicit. Round for presentation only; round required whole units upward according to the inequality.

## Operating model
Let F = monthly fixed operating costs, p = revenue per selling unit on the chosen consistent VAT basis, v = variable operating cost per unit, q = units sold/month.

- Contribution c = p - v. Include applicable transaction commissions and per-sale support/delivery costs in v, without double-counting fixed costs.
- Operating result before tax = q*c - F.
- For c > 0 and F >= 0: whole-unit break-even quantity = ceil(F/c); first whole-unit quantity with positive profit = floor(F/c) + 1. These differ when F/c is an integer.
- To achieve an adopted monthly operating-profit target T: minimum q = ceil((F+T)/c), for T >= 0. Explain whether the inequality is at least T or strictly above T.
- For c <= 0 and F > 0, no finite q achieves break-even. If c=0 and F=0, result is always zero, not positive profit. Explain any unusual negative-fixed-cost assumptions explicitly.
- Monthly total operating cost is F+q*v. Without q, report this expression rather than fabricating a total.
- Distinguish first-month new buyers, active subscribers, transactions, and repeat purchases. For subscription models, q may be active paying accounts; account for onboarding and churn separately if relevant.
- If customers buy k units/customer/month, required customers = ceil(required units/k). Do not assume k without student adoption or evidence.
- For multi-product models, use supplied/adopted sales mix and weighted contribution; otherwise show separate scenarios, not a fabricated average.

## VAT and cash
- If VAT applies at verified rate r and quoted price is gross: net sales price = gross/(1+r). If exempt, do not simply subtract VAT from revenue; check input-tax treatment. Recoverable input VAT generally should not be treated as economic expense; cash timing still matters.
- Record whether supplied cost figures include VAT and whether it is recoverable. Use a consistent provisional basis before verification; recalculate if status changes.
- One-off purchases consume cash at purchase, but an asset's expense may be depreciation; do not count both the purchase and depreciation as the same period's operating expense. Use current rules if offering tax/accounting treatment.
- Annual recurring costs / 12 is a monthly budget allocation, not necessarily the payment schedule. Deposits may tie up cash without being expenses.
- Loan principal repayment is a financing cash outflow, not operating expense; interest is separate. Loan proceeds/equity injections are not sales revenue.
- Founder drawings for a sole proprietor are not an employee salary expense. Show founder cash/living requirement separately. Employee budgets need full employer costs, verified or explicitly estimated, not net pay alone.
- A pre-tax operating result is not personal take-home pay. Separate personal taxes, SVS, remuneration, distributions, and company taxes according to the legal form. Mark simplified treatment and prevent double-counting.

## Funding need
Do not assume a three- or six-month horizon. Ask the student's horizon and current funds, or present a clearly conditional scenario.

Build period-by-period cash flows when timing matters. Required outside funds = max(0, maximum cumulative cash deficit after available own cash and committed financing, plus adopted minimum reserve). Include startup purchases/deposits, payment delays, refunds, tax/SVS payments, debt service, and founder cash requirement where appropriate. Avoid adding starting funds twice or calling unawarded grants committed financing. A simplified startup costs + months*monthly deficit estimate must be labeled a rough approximation with its timing assumptions.

## Funnel
Let N be required paying customers for the chosen period; a and b be successive conversion proportions, 0 < a,b <=1.

- Illustrative funnel: unique people reached R → qualified prospects R*a → paying customers R*a*b.
- Required unique reach = ceil(N/(a*b)). Use the product of all stage rates for more stages.
- Zero conversion implies no finite reach produces the target; missing rates imply a conditional scenario, not a forecast.
- State denominators. A conversion rate from visitors to buyers is not a rate from total impressions to buyers.
- For active subscriber targets distinguish retained customers from new acquisitions; do not funnel every retained subscriber again each month.
- Compare reach/customers only to a market estimate with compatible geography, segment, unit, and period. Multiplying visitors or impressions does not create unique people.

## Meaningful arithmetic checks
Before reporting, check with the calculation tool:
- q just below break-even loses money and q at/above the threshold meets the intended inequality.
- If F=1000, p=30, v=10: contribution=20, break-even=50, first positive-profit quantity=51.
- If 51 new buyers are needed and stage rates are .10 and .20: required reach=2550 unique people for that same period.
These are verification examples, not student defaults or market benchmarks.
