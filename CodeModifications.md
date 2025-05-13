
# Code Modifications

## Files Modified

1. **BeanStreamPayment.java**
   - Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.

2. **Stripe3Payment.java**
   - Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.

3. **StripePayment.java**
   - Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.

4. **USPSShippingQuote.java**
   - Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.

5. **PricingServiceImpl.java**
   - Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.

6. **ProductPriceUtils.java**
   - Made `getStoreFormatedAmountWithCurrency` a static method.

## Summary

The deprecated method `getAdminFormatedAmount(MerchantStore, BigDecimal)` was replaced with `getStoreFormatedAmountWithCurrency` across various files. Additionally, the `getStoreFormatedAmountWithCurrency` method was made static in the `ProductPriceUtils.java` file to improve its accessibility and usage across the codebase.