# Code Modifications

## Deprecated Method Removal

The deprecated method `getAdminFormatedAmount(com.salesmanager.core.model.merchant.MerchantStore,java.math.BigDecimal)` from the `ProductPriceUtils` class was removed and replaced with the `getStoreFormatedAmountWithCurrency` method.

## Updated Files

### Internal Callers
- **BeanStreamPayment.java**: Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.
- **PayPalRestPayment.java**: Updated commented code to use `getStoreFormatedAmountWithCurrency`.
- **Stripe3Payment.java**: Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.
- **StripePayment.java**: Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.
- **USPSShippingQuote.java**: Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.
- **PricingServiceImpl.java**: Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.

### ProductPriceUtils Class
- Made the `getStoreFormatedAmountWithCurrency` method static.

These changes ensure that the deprecated method is no longer used and that the codebase is updated to use the recommended method for formatting amounts with currency.

