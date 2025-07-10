
### Code Modifications

1. **ProductPriceUtils.java**
   - Replaced calls to `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency` in the `getFinalPrice` methods.
   - Made `getStoreFormatedAmountWithCurrency` a static method.

2. **PricingServiceImpl.java**
   - Replaced call to `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency` in the `getStringAmount` method.

3. **StripePayment.java**
   - Replaced calls to `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency` in the `authorize`, `authorizeAndCapture`, and `refund` methods.

4. **Stripe3Payment.java**
   - Replaced calls to `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency` in the `capture`, `authorizeAndCapture`, and `refund` methods.

5. **BeanStreamPayment.java**
   - Replaced calls to `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency` in the `capture`, `refund`, and `processTransaction` methods.

6. **USPSShippingQuote.java**
   - Replaced call to `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency` in the `getShippingQuotes` method.