
# Code Modifications for Deprecated Method Removal

## API Endpoints Affected
- `api/v1/private/product/{}/attribute/{}/` (PUT)
- `api/v1/private/product/{}/attribute/` (POST)
- `api/v1/cart/{}/shipping/` (POST)
- `api/v1/cart/{}/checkout/` (POST)
- `api/v1/auth/cart/{}/checkout/` (POST)
- `api/v1/private/product/{}/attribute/{}/` (GET)
- `api/v1/private/product/{}/attributes/` (GET)
- `api/v1/auth/cart/{}/shipping/` (GET)

## Internal Callers Updated
- `PricingServiceImpl.java`: Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.

## External Callers Updated
- `StripePayment.java`: Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.
- `Stripe3Payment.java`: Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.
- `BeanStreamPayment.java`: Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.
- `USPSShippingQuote.java`: Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.

## Method Made Static
- `getStoreFormatedAmountWithCurrency` in `ProductPriceUtils.java` is now a static method.

These changes ensure that the deprecated method is no longer used and the new method is utilized consistently across the codebase.