# Code Modifications

## Deprecated Method Replacement

1. **File:** `BeanStreamPayment.java`
   - Replaced `productPriceUtils.getAdminFormatedAmount(store, order.getTotal())` with `productPriceUtils.getStoreFormatedAmountWithCurrency(store, order.getTotal())`.

2. **File:** `PayPalRestPayment.java`
   - Updated commented-out code to replace `productPriceUtils.getAdminFormatedAmount(store, amount)` with `productPriceUtils.getStoreFormatedAmountWithCurrency(store, amount)`.

3. **File:** `Stripe3Payment.java`
   - Replaced all occurrences of `productPriceUtils.getAdminFormatedAmount(store, order.getTotal())` with `productPriceUtils.getStoreFormatedAmountWithCurrency(store, order.getTotal())`.

## Static Method Update

- **File:** `ProductPriceUtils.java`
  - Made the method `getStoreFormatedAmountWithCurrency` static to allow calls without an instance of `ProductPriceUtils`.

