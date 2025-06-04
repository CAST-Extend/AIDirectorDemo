# Code Modifications

## Deprecated Method Replacement

The following changes were made to replace the deprecated method `getAdminFormatedAmount(com.salesmanager.core.model.merchant.MerchantStore,java.math.BigDecimal)` with `getStoreFormatedAmountWithCurrency`:

1. **BeanStreamPayment.java**
   - Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency` at lines 94, 183, and 500.

2. **PayPalRestPayment.java**
   - Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency` at line 124.

3. **Stripe3Payment.java**
   - Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency` at lines 237, 313, and 399.

4. **StripePayment.java**
   - Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency` at lines 143, 287, and 356.

5. **USPSShippingQuote.java**
   - Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency` at line 383.

6. **PricingServiceImpl.java**
   - Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency` at line 90.

## Static Method Update

- Made the `getStoreFormatedAmountWithCurrency` method static in `ProductPriceUtils.java`.

