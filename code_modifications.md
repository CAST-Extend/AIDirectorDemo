# Code Modifications

## Deprecated Method Removal

1. **Replaced Deprecated Method Calls**
   - Updated calls to `getAdminFormatedAmount(MerchantStore store, BigDecimal amount)` to use `getStoreFormatedAmountWithCurrency(MerchantStore store, BigDecimal amount)` in the following files:
     - `BeanStreamPayment.java`
     - `PayPalRestPayment.java` (commented-out section)
     - `Stripe3Payment.java`

2. **Made Method Static**
   - Changed `getStoreFormatedAmountWithCurrency` to a static method in `ProductPriceUtils.java`.

These changes ensure that the deprecated method is no longer used and the new static method is utilized instead.
