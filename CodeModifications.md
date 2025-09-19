
### Code Modifications

1. **ProductPriceUtils.java**
   - Replaced calls to the deprecated `getAdminFormatedAmount(MerchantStore, BigDecimal)` method with `getStoreFormatedAmountWithCurrency`.
   - Made the `getStoreFormatedAmountWithCurrency` method static.

2. **PricingServiceImpl.java**
   - Updated calls to `getStoreFormatedAmountWithCurrency` to reflect its static nature by using `ProductPriceUtils.getStoreFormatedAmountWithCurrency`.