# Code Modifications

## Deprecated Method Removal

The deprecated method `getAdminFormatedAmount(com.salesmanager.core.model.merchant.MerchantStore,java.math.BigDecimal)` was removed from the following files:

1. **BeanStreamPayment.java**
   - Replaced with `getStoreFormatedAmountWithCurrency`.

2. **Stripe3Payment.java**
   - Replaced with `getStoreFormatedAmountWithCurrency`.

3. **StripePayment.java**
   - Replaced with `getStoreFormatedAmountWithCurrency`.

4. **USPSShippingQuote.java**
   - Replaced with `getStoreFormatedAmountWithCurrency`.

## Method Update

The method `getStoreFormatedAmountWithCurrency` in `ProductPriceUtils.java` was made static to facilitate its usage across the codebase.

These changes ensure that the deprecated method is no longer used and the codebase is updated to use the recommended method for formatting amounts with currency.

