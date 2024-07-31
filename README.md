# Build A Cash Register

The aim is to build a cash register app that will return change to the customer based on the price of the item, the amount of cash provided by the customer, and the amount of cash in the cash drawer.

## UX

1.  As a user, I expect an `input` element with id of `cash`.

2.  As a user, I expect a `div` dlement with id of `change-due`.

3.  As a user, I expect a `button` element with id of `purchase-btn`.

4.  As a user, if the value in the `#cash` element is less than `price`, I expect an alert to appear with the text `Customer does not have enough money to purchase the item`.

5.  As a user, if the value in the `#cash` element is equal to `price`, I expect the value in the `#change-due` element to be `No change due - customer paid with exact cash`.

6.  As a user, when `price` is `19.5` and the value in the `#cash` element is `20`, `cid` is `[
  ["PENNY", 1.01],
  ["NICKEL", 2.05],
  ["DIME", 3.1],
  ["QUARTER", 4.25],
  ["ONE", 90],
  ["FIVE", 55],
  ["TEN", 20],
  ["TWENTY", 60],
  ["ONE HUNDRED", 100]
]`, and the `#purchase-btn` element is clicked, I expect the value in the `#change-due` element to be `Status: OPEN QUARTER: $0.5`.

7.  As a user, when `price` is `3.26` and the value in the `#cash` element is `100`, `cid` is `[
  ["PENNY", 1.01],
  ["NICKEL", 2.05],
  ["DIME", 3.1],
  ["QUARTER", 4.25],
  ["ONE", 90],
  ["FIVE", 55],
  ["TEN", 20],
  ["TWENTY", 60],
  ["ONE HUNDRED", 100]
]`, and the `#purchase-btn` element is clicked, I expect the value in the `#change-due` element to be `Status: OPEN TWENTY: $60 TEN: $20 FIVE: $15 ONE: $1 QUARTER: $0.5 DIME: $0.2 PENNY: $0.04`.

8.  As a user, when `price` is `19.5` and the value in the `#cash` element is `20`, `cid` is `[
  ["PENNY", 1.01],
  ["NICKEL", 0],
  ["DIME", 0],
  ["QUARTER", 0],
  ["ONE", 0],
  ["FIVE", 0],
  ["TEN", 0],
  ["TWENTY", 0],
  ["ONE HUNDRED", 0]
]`, and the `#purchase-btn` element is clicked, I expect the value in the `#change-due` element to be `Status: INSUFFICIENT_FUNDS`.

9.  As a user, when `price` is `19.5` and the value in the `#cash` element is `20`, `cid` is `[
  ["PENNY", 1.01],
  ["NICKEL", 0],
  ["DIME", 0],
  ["QUARTER", 0],
  ["ONE", 1],
  ["FIVE", 0],
  ["TEN", 0],
  ["TWENTY", 0],
  ["ONE HUNDRED", 0]
]`, and the `#purchase-btn` element is clicked, I expect the value in the `#change-due` element to be `Status: INSUFFICIENT_FUNDS`.

10.  As a user, when `price` is `19.5` and the value in the `#cash` element is `20`, `cid` is `[
  ["PENNY", 0.5],
  ["NICKEL", 0],
  ["DIME", 0],
  ["QUARTER", 0],
  ["ONE", 0],
  ["FIVE", 0],
  ["TEN", 0],
  ["TWENTY", 0],
  ["ONE HUNDRED", 0]
]`, and the `#purchase-btn` element is clicked, I expect the value in the `#change-due` element to be `Status: CLOSED PENNY: $0.5`.

## Features

Allows the user to enter cash and to click on the purchase button.

## Technologies

Uses HTML5, CSS3 and JavaScript.

## Testing

Ensure all user stories have been met.  Change the values of `price` and `cid` in `script.js`.

## Deployment

Deployed on [GitHub Pages](https://derektypist.github.io/build-a-cash-register/) at the main branch.

## Credits

### Acknowledgements

[FreeCodeCamp - Cash Register](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures-v8/build-a-cash-register-project/build-a-cash-register)


