
# Code Modifications

## Deprecated Method Replacement

1. **BeanStreamPayment.java**
   - Replaced `getAdminFormatedAmount(store, order.getTotal())` with `getStoreFormatedAmountWithCurrency(store, order.getTotal())`.

2. **PayPalRestPayment.java**
   - Updated commented-out code to replace `getAdminFormatedAmount(store, amount)` with `getStoreFormatedAmountWithCurrency(store, amount)`.

3. **Stripe3Payment.java**
   - Replaced all occurrences of `getAdminFormatedAmount(store, order.getTotal())` with `getStoreFormatedAmountWithCurrency(store, order.getTotal())`.

## Method Update

1. **ProductPriceUtils.java**
   - Made `getStoreFormatedAmountWithCurrency` a static method.