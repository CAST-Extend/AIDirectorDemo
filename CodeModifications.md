# Code Modifications

## Changes Made

1. **Made `getStoreFormatedAmountWithCurrency` Static**
   - Updated the `ProductPriceUtils.java` file to make the `getStoreFormatedAmountWithCurrency` method static.

2. **Checked for Deprecated Method Usage**
   - Searched the repository for any usage of the deprecated `getAdminFormatedAmount(MerchantStore, BigDecimal)` method.
   - No direct calls to the deprecated method were found, indicating it might have already been replaced elsewhere.

These changes address the tech debt by ensuring the deprecated method is no longer used and the recommended method is static for better utility access.

