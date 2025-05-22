
# Code Modifications

The following changes were made to address the tech debt of removing the deprecated method `getAdminFormatedAmount(com.salesmanager.core.model.merchant.MerchantStore,java.math.BigDecimal)`:

1. **PricingServiceImpl.java**
   - Replaced the call to `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency` in the `getStringAmount` method.

2. **StripePayment.java**
   - Replaced all calls to `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency` in the `authorize`, `authorizeAndCapture`, and `refund` methods.

3. **Stripe3Payment.java**
   - Replaced all calls to `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency` in the `capture`, `authorizeAndCapture`, and `refund` methods.

4. **BeanStreamPayment.java**
   - Replaced all calls to `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency` in the `capture`, `refund`, and `processTransaction` methods.

5. **USPSShippingQuote.java**
   - Replaced the call to `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency` in the `getShippingQuotes` method.

6. **ProductPriceUtils.java**
   - Made the `getStoreFormatedAmountWithCurrency` method static.