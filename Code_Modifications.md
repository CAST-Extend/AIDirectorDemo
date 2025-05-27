
### Code Modifications

1. **PricingServiceImpl.java**
   - Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.

2. **StripePayment.java**
   - Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.

3. **Stripe3Payment.java**
   - Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.

4. **BeanStreamPayment.java**
   - Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.

5. **USPSShippingQuote.java**
   - Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.

6. **ProductPriceUtils.java**
   - Made `getStoreFormatedAmountWithCurrency` a static method.