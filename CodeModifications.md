# Code Modifications

## Changes in ProductPriceUtils.java

- Made the `getStoreFormatedAmountWithCurrency` method static.
- This change allows the method to be called without an instance of the `ProductPriceUtils` class.

These changes were made to address the tech debt of removing the usage of the deprecated method `getAdminFormatedAmount` and to improve the utility of the `getStoreFormatedAmountWithCurrency` method.
## Changes in BeanStreamPayment.java

- Replaced calls to the deprecated `getAdminFormatedAmount` method with the static `getStoreFormatedAmountWithCurrency` method.

## Changes in Stripe3Payment.java

- Replaced calls to the deprecated `getAdminFormatedAmount` method with the static `getStoreFormatedAmountWithCurrency` method.

These changes ensure that the codebase no longer relies on the deprecated method and utilizes the updated static method for formatting amounts with currency.

