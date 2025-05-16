# Code Modifications for Deprecated Method Removal

## Files Modified

1. **PricingServiceImpl.java**
   - Replaced `getAdminFormatedAmount(store, amount)` with `getStoreFormatedAmountWithCurrency(store, amount)`.

2. **StripePayment.java**
   - Replaced all instances of `getAdminFormatedAmount(store, amount)` with `getStoreFormatedAmountWithCurrency(store, amount)`.

3. **Stripe3Payment.java**
   - Replaced all instances of `getAdminFormatedAmount(store, amount)` with `getStoreFormatedAmountWithCurrency(store, amount)`.

4. **BeanStreamPayment.java**
   - Replaced all instances of `getAdminFormatedAmount(store, amount)` with `getStoreFormatedAmountWithCurrency(store, amount)`.

## Method Changes

- **ProductPriceUtils.java**
  - Made `getStoreFormatedAmountWithCurrency` a static method.

These changes ensure that the deprecated method `getAdminFormatedAmount` is no longer used and the new method `getStoreFormatedAmountWithCurrency` is utilized instead. The static modification allows for easier access without needing an instance of `ProductPriceUtils`.

