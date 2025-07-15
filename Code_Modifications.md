
# Code Modifications

## Files Modified

1. **BeanStreamPayment.java**
   - Replaced `getAdminFormatedAmount(store, order.getTotal())` with `getStoreFormatedAmountWithCurrency(store, order.getTotal())`.

2. **PayPalRestPayment.java**
   - Updated commented-out code to replace `getAdminFormatedAmount(store, amount)` with `getStoreFormatedAmountWithCurrency(store, amount)`.

3. **Stripe3Payment.java**
   - Replaced all occurrences of `getAdminFormatedAmount(store, order.getTotal())` with `getStoreFormatedAmountWithCurrency(store, order.getTotal())`.

4. **ProductPriceUtils.java**
   - Made the `getStoreFormatedAmountWithCurrency` method static.

These changes were made to remove the usage of the deprecated method `getAdminFormatedAmount` and replace it with the updated static method `getStoreFormatedAmountWithCurrency`. This ensures that the codebase is up-to-date and avoids using deprecated methods.