
### Code Modifications

1. **PricingServiceImpl.java**
   - Replaced `getAdminFormatedAmount(store, amount)` with `getStoreFormatedAmountWithCurrency(store, amount)`.

2. **StripePayment.java**
   - Replaced all occurrences of `getAdminFormatedAmount(store, amount)` with `getStoreFormatedAmountWithCurrency(store, amount)`.

3. **Stripe3Payment.java**
   - Replaced all occurrences of `getAdminFormatedAmount(store, amount)` with `getStoreFormatedAmountWithCurrency(store, amount)`.

4. **BeanStreamPayment.java**
   - Replaced all occurrences of `getAdminFormatedAmount(store, amount)` with `getStoreFormatedAmountWithCurrency(store, amount)`.

5. **USPSShippingQuote.java**
   - Replaced `getAdminFormatedAmount(store, orderTotal)` with `getStoreFormatedAmountWithCurrency(store, orderTotal)`.

6. **ProductPriceUtils.java**
   - Made `getStoreFormatedAmountWithCurrency` a static method.