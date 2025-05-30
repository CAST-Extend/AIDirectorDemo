
# Code Modifications

## Deprecated Method Replacement

The following changes were made to replace the deprecated method `getAdminFormatedAmount(com.salesmanager.core.model.merchant.MerchantStore,java.math.BigDecimal)` with `getStoreFormatedAmountWithCurrency`:

1. **BeanStreamPayment.java**
   - Replaced all occurrences of `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.

2. **Stripe3Payment.java**
   - Replaced all occurrences of `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.

3. **StripePayment.java**
   - Replaced all occurrences of `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.

4. **USPSShippingQuote.java**
   - Replaced the occurrence of `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.

5. **PricingServiceImpl.java**
   - Replaced the occurrence of `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.

## Method Update

- The `getStoreFormatedAmountWithCurrency` method in `ProductPriceUtils.java` was updated to be a static method to allow for static access.