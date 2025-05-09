
# Code Modifications

## ProductPriceUtils.java
- Made the `getStoreFormatedAmountWithCurrency` method static.

## PricingServiceImpl.java
- Replaced the call to the deprecated `getAdminFormatedAmount(MerchantStore, BigDecimal)` method with the static `getStoreFormatedAmountWithCurrency` method in the `getStringAmount` method.