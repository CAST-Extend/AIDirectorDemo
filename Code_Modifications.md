
### Code Modifications

1. **ProductPriceUtils.java**
   - Made the `getStoreFormatedAmountWithCurrency` method static.

2. **PricingServiceImpl.java**
   - Replaced calls to the deprecated `getAdminFormatedAmount` method with `getStoreFormatedAmountWithCurrency`.

3. **StripePayment.java**
   - Replaced calls to the deprecated `getAdminFormatedAmount` method with `getStoreFormatedAmountWithCurrency`.

4. **Stripe3Payment.java**
   - Replaced calls to the deprecated `getAdminFormatedAmount` method with `getStoreFormatedAmountWithCurrency`.

5. **BeanStreamPayment.java**
   - Replaced calls to the deprecated `getAdminFormatedAmount` method with `getStoreFormatedAmountWithCurrency`.

6. **USPSShippingQuote.java**
   - Replaced calls to the deprecated `getAdminFormatedAmount` method with `getStoreFormatedAmountWithCurrency`.