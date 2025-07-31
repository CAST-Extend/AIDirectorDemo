### Code Modifications

1. **Replaced Deprecated Method Calls**:
   - Replaced all calls to the deprecated method `getAdminFormatedAmount(MerchantStore store, BigDecimal amount)` with `getStoreFormatedAmountWithCurrency(MerchantStore store, BigDecimal amount)` in the following files:
     - `PricingServiceImpl.java`
     - `StripePayment.java`
     - `Stripe3Payment.java`
     - `BeanStreamPayment.java`
     - `USPSShippingQuote.java`

2. **Made Method Static**:
   - Made the `getStoreFormatedAmountWithCurrency(MerchantStore store, BigDecimal amount)` method static in the `ProductPriceUtils.java` file.

These changes ensure that the deprecated method is no longer used and the new method is utilized consistently across the codebase.

