# Code Modifications

## Changes Made:

1. **ProductPriceUtils.java**
   - Made the `getStoreFormatedAmountWithCurrency` method static.

2. **BeanStreamPayment.java**
   - Replaced calls to `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.

3. **PayPalRestPayment.java**
   - Updated commented-out code to use `getStoreFormatedAmountWithCurrency` instead of `getAdminFormatedAmount`.

4. **Stripe3Payment.java**
   - Replaced calls to `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.

5. **StripePayment.java**
   - Replaced calls to `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.

6. **USPSShippingQuote.java**
   - Replaced calls to `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.

7. **PricingServiceImpl.java**
   - Replaced calls to `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.

