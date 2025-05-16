# Code Modifications

## Deprecated Method Replacement
- Replaced all occurrences of the deprecated method `getAdminFormatedAmount(MerchantStore store, BigDecimal amount)` with `getStoreFormatedAmountWithCurrency(store, amount)` in the `ProductPriceUtils.java` file.

## Static Method Update
- Made the `getStoreFormatedAmountWithCurrency(MerchantStore store, BigDecimal amount)` method static in the `ProductPriceUtils.java` file.

These changes ensure that the deprecated method is no longer used and the new method is accessible as a static utility function.

