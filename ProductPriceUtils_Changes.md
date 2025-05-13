
# ProductPriceUtils Changes

## Modifications Made

1. **Made Method Static**: The `getStoreFormatedAmountWithCurrency` method in `ProductPriceUtils.java` was made static to align with the task requirements.

2. **Deprecated Method Usage**: The usage of the deprecated method `getAdminFormatedAmount(MerchantStore, BigDecimal)` was identified for removal, although no direct calls were found in the current repository search.

## Next Steps

- Ensure that any future calls to `getAdminFormatedAmount(MerchantStore, BigDecimal)` are replaced with `getStoreFormatedAmountWithCurrency`.
- Conduct tests to verify that the static method change does not impact existing functionality.