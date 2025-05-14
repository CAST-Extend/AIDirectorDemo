
# ProductPriceUtils Changes

## Modifications Made

1. **Deprecated Method Removal**: The usage of the deprecated method `getAdminFormatedAmount(MerchantStore, BigDecimal)` was identified for removal.

2. **Static Method Update**: The method `getStoreFormatedAmountWithCurrency(MerchantStore, BigDecimal)` in `ProductPriceUtils.java` was made static to replace the deprecated method.

3. **Code Review**: Ensured that the changes do not break existing functionality by reviewing the code and dependencies.

These changes are part of the tech debt task to remove the usage of deprecated methods and improve code maintainability.