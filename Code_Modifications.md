
# Code Modifications

## Deprecated Method Removal

The deprecated method `getAdminFormatedAmount(com.salesmanager.core.model.merchant.MerchantStore,java.math.BigDecimal)` was removed from the following files:

1. **BeanStreamPayment.java**
   - Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency` in three places.

2. **PayPalRestPayment.java**
   - The usage was within a commented-out block, so no active changes were made.

3. **Stripe3Payment.java**
   - Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency` in three places.

4. **StripePayment.java**
   - Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency` in three places.

5. **USPSShippingQuote.java**
   - Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency` in one place.

6. **PricingServiceImpl.java**
   - Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency` in one place.

## Method Update

- The method `getStoreFormatedAmountWithCurrency` in `ProductPriceUtils.java` was updated to be a static method.

These changes ensure that the deprecated method is no longer used and the new method is utilized consistently across the codebase.