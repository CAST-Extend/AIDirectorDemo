# Code Modifications

## Deprecated Method Replacement

The deprecated method `getAdminFormatedAmount(com.salesmanager.core.model.merchant.MerchantStore,java.math.BigDecimal)` was replaced with `getStoreFormatedAmountWithCurrency` in the following files:

1. **BeanStreamPayment.java**
   - Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency` in `capture`, `refund`, and `processTransaction` methods.

2. **Stripe3Payment.java**
   - Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency` in `capture`, `authorizeAndCapture`, and `refund` methods.

3. **StripePayment.java**
   - Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency` in `authorize`, `authorizeAndCapture`, and `refund` methods.

4. **USPSShippingQuote.java**
   - Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency` in `getShippingQuotes` method.

5. **PricingServiceImpl.java**
   - Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency` in `getStringAmount` method.

## Static Method Update

The method `getStoreFormatedAmountWithCurrency` in `ProductPriceUtils.java` was updated to be a static method. All calls to this method were updated to use the class name `ProductPriceUtils` instead of an instance.


