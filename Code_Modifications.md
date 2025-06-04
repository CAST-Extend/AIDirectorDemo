### Code Modifications

1. **ProductPriceUtils.java**
   - Replaced calls to `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.
   - Made `getStoreFormatedAmountWithCurrency` method static.

2. **PricingServiceImpl.java**
   - Replaced call to `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.

3. **StripePayment.java**
   - Replaced calls to `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.

4. **Stripe3Payment.java**
   - Replaced calls to `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.

5. **BeanStreamPayment.java**
   - Replaced calls to `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.

6. **USPSShippingQuote.java**
   - Replaced call to `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.

