# Code Modifications

## Deprecated Method Replacement

The following changes were made to replace the deprecated method `getAdminFormatedAmount(com.salesmanager.core.model.merchant.MerchantStore,java.math.BigDecimal)` with the static method `getStoreFormatedAmountWithCurrency`:

1. **BeanStreamPayment.java**
   - Replaced `productPriceUtils.getAdminFormatedAmount` with `ProductPriceUtils.getStoreFormatedAmountWithCurrency`.

2. **PayPalRestPayment.java**
   - Replaced `productPriceUtils.getAdminFormatedAmount` with `ProductPriceUtils.getStoreFormatedAmountWithCurrency` in a commented-out section.

3. **Stripe3Payment.java**
   - Replaced `productPriceUtils.getAdminFormatedAmount` with `ProductPriceUtils.getStoreFormatedAmountWithCurrency`.

4. **StripePayment.java**
   - Replaced `productPriceUtils.getAdminFormatedAmount` with `ProductPriceUtils.getStoreFormatedAmountWithCurrency`.

5. **USPSShippingQuote.java**
   - Replaced `productPriceUtils.getAdminFormatedAmount` with `ProductPriceUtils.getStoreFormatedAmountWithCurrency`.

6. **PricingServiceImpl.java**
   - Replaced `priceUtil.getAdminFormatedAmount` with `ProductPriceUtils.getStoreFormatedAmountWithCurrency`.

## Method Update

- Made `getStoreFormatedAmountWithCurrency` a static method in `ProductPriceUtils.java`.

