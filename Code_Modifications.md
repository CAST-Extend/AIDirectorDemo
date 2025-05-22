
### Code Modifications

1. **PricingServiceImpl.java**
   - Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.

2. **StripePayment.java**
   - Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency` in methods `authorize`, `authorizeAndCapture`, and `refund`.

3. **Stripe3Payment.java**
   - Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency` in methods `capture`, `authorizeAndCapture`, and `refund`.

4. **BeanStreamPayment.java**
   - Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency` in methods `capture`, `refund`, and `processTransaction`.

5. **USPSShippingQuote.java**
   - Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency` in method `getShippingQuotes`.

6. **ProductPriceUtils.java**
   - Made `getStoreFormatedAmountWithCurrency` a static method.