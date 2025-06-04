
### Code Modifications for Removing Deprecated Method Usage

1. **Updated `PricingServiceImpl.java`:**
   - Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency` in the `getStringAmount` method.

2. **Updated `StripePayment.java`:**
   - Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency` in the `authorize`, `authorizeAndCapture`, and `refund` methods.

3. **Updated `Stripe3Payment.java`:**
   - Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency` in the `capture`, `authorizeAndCapture`, and `refund` methods.

4. **Updated `BeanStreamPayment.java`:**
   - Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency` in the `capture`, `refund`, and `processTransaction` methods.

5. **Updated `USPSShippingQuote.java`:**
   - Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency` in the `getShippingQuotes` method.

6. **Updated `ProductPriceUtils.java`:**
   - Made `getStoreFormatedAmountWithCurrency` a static method.