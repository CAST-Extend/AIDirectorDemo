
# Code Modifications

## Overview
This document outlines the changes made to remove the usage of the deprecated method `getAdminFormatedAmount(MerchantStore store, BigDecimal amount)` from the `ProductPriceUtils` Java class and replace it with `getStoreFormatedAmountWithCurrency`.

## Changes Made

### 1. `ProductPriceUtils.java`
- **Modification**: Made the `getStoreFormatedAmountWithCurrency` method static.
- **Rationale**: To allow the method to be called without an instance of `ProductPriceUtils`.

### 2. `PricingServiceImpl.java`
- **Modification**: Replaced the call to `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency` in the `getStringAmount` method.
- **Rationale**: To use the updated method for formatting amounts with currency.

### 3. `StripePayment.java`
- **Modification**: Replaced calls to `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency` in the `authorize`, `authorizeAndCapture`, and `refund` methods.
- **Rationale**: To ensure the correct method is used for formatting amounts with currency.

### 4. `Stripe3Payment.java`
- **Modification**: Replaced calls to `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency` in the `capture`, `authorizeAndCapture`, and `refund` methods.
- **Rationale**: To ensure the correct method is used for formatting amounts with currency.

### 5. `BeanStreamPayment.java`
- **Modification**: Replaced calls to `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency` in the `capture`, `refund`, and `processTransaction` methods.
- **Rationale**: To ensure the correct method is used for formatting amounts with currency.

### 6. `USPSShippingQuote.java`
- **Modification**: Replaced the call to `getAdminFormatedAmount` with `getStoreFormatedAmountWithCurrency` in the `getShippingQuotes` method.
- **Rationale**: To ensure the correct method is used for formatting amounts with currency.

## Conclusion
These changes ensure that the deprecated method is no longer used and that the updated method is utilized consistently across the codebase. This helps maintain code quality and future-proofing against deprecated functionality.