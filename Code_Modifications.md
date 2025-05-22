
# Code Modifications

## Deprecated Method Replacement

The deprecated method `getAdminFormatedAmount(com.salesmanager.core.model.merchant.MerchantStore,java.math.BigDecimal)` was replaced with `getStoreFormatedAmountWithCurrency` in the following files:

1. **BeanStreamPayment.java**
   - Replaced 3 occurrences of the deprecated method.

2. **PayPalRestPayment.java**
   - Replaced 1 occurrence of the deprecated method.

3. **Stripe3Payment.java**
   - Replaced 3 occurrences of the deprecated method.

4. **StripePayment.java**
   - Replaced 3 occurrences of the deprecated method.

5. **USPSShippingQuote.java**
   - Replaced 1 occurrence of the deprecated method.

6. **PricingServiceImpl.java**
   - Replaced 1 occurrence of the deprecated method.

## Static Method Update

The method `getStoreFormatedAmountWithCurrency` in `ProductPriceUtils.java` was made static to facilitate its usage across the application.

---

These changes ensure that the deprecated method is no longer used and the new method is accessible as a static utility function.