# Code Modifications

## Deprecated Method Replacement

The following changes were made to replace the deprecated method `getAdminFormatedAmount(com.salesmanager.core.model.merchant.MerchantStore,java.math.BigDecimal)` with `getStoreFormatedAmountWithCurrency`:

1. **BeanStreamPayment.java**
   - Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.
   - Updated method calls to use static context.

2. **PayPalRestPayment.java**
   - Updated commented-out usage of `getAdminFormatedAmount` to `getStoreFormatedAmountWithCurrency`.

3. **Stripe3Payment.java**
   - Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.
   - Updated method calls to use static context.

4. **StripePayment.java**
   - Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.
   - Updated method calls to use static context.

5. **USPSShippingQuote.java**
   - Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.
   - Updated method calls to use static context.

6. **PricingServiceImpl.java**
   - Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.
   - Updated method calls to use static context.

## Method Update

- Made `getStoreFormatedAmountWithCurrency` a static method in `ProductPriceUtils.java`.

