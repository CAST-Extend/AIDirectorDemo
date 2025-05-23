
### Code Modifications

1. **PricingServiceImpl.java**
   - Updated `getStringAmount` method to use `getStoreFormatedAmountWithCurrency` instead of the deprecated `getAdminFormatedAmount`.

2. **StripePayment.java**
   - Updated `authorize`, `authorizeAndCapture`, and `refund` methods to use `getStoreFormatedAmountWithCurrency` instead of the deprecated `getAdminFormatedAmount`.

3. **Stripe3Payment.java**
   - Updated `capture`, `authorizeAndCapture`, and `refund` methods to use `getStoreFormatedAmountWithCurrency` instead of the deprecated `getAdminFormatedAmount`.

4. **BeanStreamPayment.java**
   - Updated `capture`, `refund`, and `processTransaction` methods to use `getStoreFormatedAmountWithCurrency` instead of the deprecated `getAdminFormatedAmount`.

5. **USPSShippingQuote.java**
   - Updated `getShippingQuotes` method to use `getStoreFormatedAmountWithCurrency` instead of the deprecated `getAdminFormatedAmount`.

6. **ProductPriceUtils.java**
   - Made `getStoreFormatedAmountWithCurrency` method static.