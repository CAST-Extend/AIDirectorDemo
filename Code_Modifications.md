
# Code Modifications

## Deprecated Method Replacement

1. **BeanStreamPayment.java**
   - Replaced `getAdminFormatedAmount(store, order.getTotal())` with `getStoreFormatedAmountWithCurrency(store, order.getTotal())`.

2. **PayPalRestPayment.java**
   - Replaced `getAdminFormatedAmount(store, amount)` with `getStoreFormatedAmountWithCurrency(store, amount)`.

3. **Stripe3Payment.java**
   - Replaced `getAdminFormatedAmount(store, order.getTotal())` with `getStoreFormatedAmountWithCurrency(store, order.getTotal())`.

4. **StripePayment.java**
   - Replaced `getAdminFormatedAmount(store, amount)` with `getStoreFormatedAmountWithCurrency(store, amount)`.

5. **USPSShippingQuote.java**
   - Replaced `getAdminFormatedAmount(store, orderTotal)` with `getStoreFormatedAmountWithCurrency(store, orderTotal)`.

6. **PricingServiceImpl.java**
   - Replaced `getAdminFormatedAmount(store, amount)` with `getStoreFormatedAmountWithCurrency(store, amount)`.

## Method Modification

- **ProductPriceUtils.java**
  - Made `getStoreFormatedAmountWithCurrency` a static method.