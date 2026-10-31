```sankey
width: 900
height: 650
margin:
  top: 20
  right: 180
  bottom: 20
  left: 20

nodes:
  - name: Wages
  - name: Budget
  - name: Income Tax
  - name: Savings
  - name: Housing
  - name: Car
  - name: Food
  - name: Entertainment
  - name: Health
  - name: State/Local Tax
  - name: FICA
  - name: Fed Tax
  - name: Investments
  - name: Checking
  - name: 403b pre-tax
  - name: 403b Roth
  - name: Rent
  - name: Internet/Cable
  - name: Electric
  - name: Laundry
  - name: Groceries
  - name: Restaurants
  - name: Alcohol
  - name: Car Loan
  - name: Gas
  - name: Disability Benefits

links:
  - source: Wages
    target: Budget
    value: 7083
  - source: Budget
    target: Income Tax
    value: 1495
  - source: Budget
    target: Savings
    value: 3429
  - source: Budget
    target: Housing
    value: 1336
  - source: Budget
    target: Car
    value: 407
  - source: Budget
    target: Food
    value: 280
  - source: Budget
    target: Entertainment
    value: 100
  - source: Budget
    target: Health
    value: 36
  - source: Income Tax
    target: State/Local Tax
    value: 329
  - source: Income Tax
    target: FICA
    value: 542
  - source: Income Tax
    target: Fed Tax
    value: 624
  - source: Savings
    target: Investments
    value: 2993
  - source: Savings
    target: Checking
    value: 436
  - source: Investments
    target: 403b pre-tax
    value: 1505
  - source: Investments
    target: 403b Roth
    value: 1488
  - source: Housing
    target: Rent
    value: 1204
  - source: Housing
    target: Internet/Cable
    value: 40
  - source: Housing
    target: Electric
    value: 80
  - source: Housing
    target: Laundry
    value: 12
  - source: Food
    target: Groceries
    value: 150
  - source: Food
    target: Restaurants
    value: 100
  - source: Food
    target: Alcohol
    value: 30
  - source: Car
    target: Car Loan
    value: 327
  - source: Car
    target: Gas
    value: 80
  - source: Health
    target: Disability Benefits
    value: 36
```

### SankeyMatic Archive
Wages [7083] Budget

Budget [1495] Income Tax
Budget [3429] Savings
Budget [1336] Housing
Budget [407] Car
Budget [280] Food
Budget [100] Entertainment
Budget [36] Health

Income Tax [329] State/Local Tax
Income Tax [542] FICA
Income Tax [624] Fed Tax

Savings [2993] Investments
Savings [436] Checking

Investments [1505] 403b pre-tax
Investments [1488] 403b Roth
// Investments [0] 457b pre-tax
// Investments [0] 457b Roth
// Investments [0] Roth IRA
// Investments [0] Personal Stocks

Housing [1204] Rent
Housing [40] Internet/Cable
Housing [80] Electric
Housing [12] Laundry

Food [150] Groceries
Food [100] Restaurants
Food [30] Alcohol

Car [327] Car Loan
Car [80] Gas

Health [36] Disability Benefits