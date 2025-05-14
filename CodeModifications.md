# Code Modifications

## Changes Made to ProductPriceUtils.java

1. **Made Method Static**: The method `getStoreFormatedAmountWithCurrency(MerchantStore store, BigDecimal amount)` was made static to allow for its usage without instantiating the `ProductPriceUtils` class.

These changes were made to address the tech debt of removing the usage of the deprecated method `getAdminFormatedAmount(MerchantStore, BigDecimal)` and replacing it with the static method `getStoreFormatedAmountWithCurrency`.
