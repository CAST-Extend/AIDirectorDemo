# Code Modifications

## Deprecated Method Removal

1. **File:** `BeanStreamPayment.java`
   - Replaced `getAdminFormatedAmount(store, order.getTotal())` with `getStoreFormatedAmountWithCurrency(store, order.getTotal())`.

2. **File:** `Stripe3Payment.java`
   - Replaced `getAdminFormatedAmount(store, order.getTotal())` with `getStoreFormatedAmountWithCurrency(store, order.getTotal())`.

## Static Method Update

1. **File:** `ProductPriceUtils.java`
   - Made `getStoreFormatedAmountWithCurrency` method static.

These changes ensure that the deprecated method is no longer used and the new static method is utilized instead.

