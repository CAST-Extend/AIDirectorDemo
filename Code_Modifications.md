
### Code Modifications for Removing Deprecated Method Usage

1. **PricingServiceImpl.java**
   - Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency` in the `getStringAmount` method.

2. **StripePayment.java**
   - Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency` in the `authorize`, `authorizeAndCapture`, and `refund` methods.

3. **Stripe3Payment.java**
   - Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency` in the `capture`, `authorizeAndCapture`, and `refund` methods.

4. **BeanStreamPayment.java**
   - Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency` in the `capture`, `refund`, and `processTransaction` methods.

5. **USPSShippingQuote.java**
   - Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency` in the `getShippingQuotes` method.

6. **ProductPriceUtils.java**
   - Made `getStoreFormatedAmountWithCurrency` a static method.