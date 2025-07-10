
# Tech Debt Removal Documentation

## Overview
This document outlines the changes made to remove the usage of the deprecated method `getAdminFormatedAmount(com.salesmanager.core.model.merchant.MerchantStore,java.math.BigDecimal)` from the `ProductPriceUtils` Java class.

## API Endpoints Updated
- **BeanStreamPayment.java**: Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.
- **PayPalRestPayment.java**: Updated commented-out usage of `getAdminFormatedAmount`.
- **Stripe3Payment.java**: Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.
- **StripePayment.java**: Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.
- **USPSShippingQuote.java**: Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.

## Internal Callers Updated
- **PricingServiceImpl.java**: Replaced `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency`.

## Modifications to ProductPriceUtils
- Made the `getStoreFormatedAmountWithCurrency` method static.

## Conclusion
All occurrences of the deprecated method have been successfully replaced, and the necessary method in `ProductPriceUtils` has been updated to static. This ensures that the codebase no longer relies on deprecated functionality and adheres to current best practices.