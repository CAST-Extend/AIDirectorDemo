
# Code Modifications

## Deprecated Method Replacement

The following changes were made to replace the deprecated method `getAdminFormatedAmount(com.salesmanager.core.model.merchant.MerchantStore,java.math.BigDecimal)` with `getStoreFormatedAmountWithCurrency`:

1. **BeanStreamPayment.java**
   - Replaced `productPriceUtils.getAdminFormatedAmount(store, order.getTotal())` with `ProductPriceUtils.getStoreFormatedAmountWithCurrency(store, order.getTotal())`.

2. **PayPalRestPayment.java**
   - Replaced `productPriceUtils.getAdminFormatedAmount(store, amount)` with `ProductPriceUtils.getStoreFormatedAmountWithCurrency(store, amount)`.

3. **Stripe3Payment.java**
   - Replaced `productPriceUtils.getAdminFormatedAmount(store, order.getTotal())` with `ProductPriceUtils.getStoreFormatedAmountWithCurrency(store, order.getTotal())`.

4. **StripePayment.java**
   - Replaced `productPriceUtils.getAdminFormatedAmount(store, amount)` with `ProductPriceUtils.getStoreFormatedAmountWithCurrency(store, amount)`.

5. **USPSShippingQuote.java**
   - Replaced `productPriceUtils.getAdminFormatedAmount(store, orderTotal)` with `ProductPriceUtils.getStoreFormatedAmountWithCurrency(store, orderTotal)`.

6. **PricingServiceImpl.java**
   - Replaced `priceUtil.getAdminFormatedAmount(store, amount)` with `ProductPriceUtils.getStoreFormatedAmountWithCurrency(store, amount)`.

## Static Method Update

- The method `getStoreFormatedAmountWithCurrency` in `ProductPriceUtils.java` was made static.

## Method Call Updates

- Updated all method calls to `getStoreFormatedAmountWithCurrency` to use the static context `ProductPriceUtils.getStoreFormatedAmountWithCurrency` in the following files:
  - BeanStreamPayment.java
  - PayPalRestPayment.java
  - Stripe3Payment.java
  - StripePayment.java
  - USPSShippingQuote.java
  - PricingServiceImpl.java