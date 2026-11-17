# Shop Payroll Demo

A small React Native demo for managing shop employees, sales, and monthly pay.

## What it does

- Add an employee.
- Enter monthly salary.
- Set the employee's commission percentage.
- Record who made each sale.
- Enter the sale amount and the profit from that sale.
- Set a different commission percentage for each employee.
- See total pay for each employee.
- See the full payroll total.

## Payroll rule

```text
employee commission = profit from that employee's sales × their commission rate
total pay = monthly salary + commission
```

The employee receives their percentage of profit, not of the full sale amount. For example, a $12,000 sale with $3,000 profit gives a 5% employee $150 commission. Each employee can have a different rate.

The app checks that profit is not greater than the sale amount, commission stays between 0% and 100%, and commission never exceeds profit.

The app stores employee data locally on the device. It is a demo and does not include login, tax calculation, bank payments, or server storage.

## Run it

```bash
npm install
npm start
npm run android
```

Checks:

```bash
npm run type-check
npm test -- --runInBand
```
# PayRollDemo
