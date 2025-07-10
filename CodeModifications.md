
### Code Modifications

1. **Replaced Deprecated Method Calls**:
   - Replaced calls to `getAdminFormatedAmount(MerchantStore store, BigDecimal amount)` with `getStoreFormatedAmountWithCurrency(MerchantStore store, BigDecimal amount)` in the following files:
     - `PricingServiceImpl.java`
     - `StripePayment.java`
     - `Stripe3Payment.java`
     - `BeanStreamPayment.java`
     - `USPSShippingQuote.java`

2. **Made Method Static**:
   - Updated the `getStoreFormatedAmountWithCurrency` method in `ProductPriceUtils.java` to be static.

These changes ensure that the deprecated method is no longer used and the new method can be called without an instance of the class.