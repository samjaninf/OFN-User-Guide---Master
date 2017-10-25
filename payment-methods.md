# Payment methods

You must set up payment methods before you can open an order cycle.

%accordion%Accessing payment methods%accordion%

Click **Enterprises **in the blue horizontal menu, and then click **Manage **next to your enterprise. Then, click Payment methods in the menu on the left hand side.

[![](https://openfoodnetwork.org/wp-content/uploads/2015/05/Access-demo-hub-profile-edit.png "Access demo hub profile edit")](https://openfoodnetwork.org/wp-content/uploads/2015/05/Access-demo-hub-profile-edit.png)

%/accordion%

## Creating a new payment method

Click on the **create new payment method **button.

Then, the first step in setting up a Payment Method is to tick your enterprise, in the box on the right hand side of the page titled Hubs.  This indicates that the payment method you are about to create will apply to your enterprise.

**Name:** Choose a name for this payment method. \(i.e. Pay with credit card using Paypal, Cash on delivery or Bank Transfer etc\). It will be displayed at checkout and on customers' order confirmation emails.

**Description:** Here you can provide further details about the payment method. For example, for a bank transfer, you would provide details of the bank account. This description will be displayed at checkout and in order confirmation emails. An screenshot showing how a payment method displays at checkout is shown below. The customer has selected ‘cash on collection/delivery’ and the ‘correct change…’ description is displayed.

![](https://openfoodnetwork.org/wp-content/uploads/2015/05/Payment-at-checkout.png "Payment message displayed at checkout")

**Active: **Select whether this payment method is currently visible and available, or not.

**Tags:** You can use tag rules to make certain payment methods available/unavailable for specific customers \(e.g. wholesale vs retail\). See [here](/customer-accounts-and-tagging.md) for details.

**Provider: **There are five provider options. Select the one which is relevant to the payment method you are creating.

1. MasterCard Internet Gateway Service \(MIGS\)
2. PayPal Express
3. [Pin Payments](https://pin.net.au/)
4. Cash/EFT/etc. \(this is for payments which do not require automatic validation\)
5. Stripe

If you have selected ‘Cash/EFT/etc..’ as the provider, click **Create** to end the process.

For MasterCard, Paypal and Pin Payments additional instructions are below.

### PayPal

To setup a PayPal payment method, you need a PayPal business or merchant account. You can create one [here](https://www.paypal.com/au/webapps/mpp/merchant). Once you have that, you can set up ‘API access’ within PayPal, which will enable OFN to connect customers directly with your PayPal account.

1. Login to your PayPal Account

2. Click Tools and then select API credentials

[![](https://openfoodnetwork.org/wp-content/uploads/2015/05/Paypal-tools-API-credentials.png "Paypal tools API credentials")](https://openfoodnetwork.org/wp-content/uploads/2015/05/Paypal-tools-API-credentials.png)

1. Click on ‘View API Signature’  and you will see the API details you’ll need to set up Paypal in OFN.

![](https://openfoodnetwork.org/wp-content/uploads/2015/05/API-Access.png "API Access")

![](https://openfoodnetwork.org/wp-content/uploads/2015/05/Api-Signature.png "Api Signature")

1. In OFN, make sure you are logged in as your Enterprise User. Go to an Enterprise and create a Payment Method. Select PayPal and fill in the details from the PayPal site.

**Login:**Type the API Username.

**Password:**Type the API Password.

**Signature:**Type the Signature  in this field.

![](https://openfoodnetwork.org/wp-content/uploads/2015/05/New-Payment-Paypal-1.png "New Payment Paypal")

**Server**

Change the ‘server’ field to ‘live’ – this is case sensitive.

**Solution**

Solution determines whether or not a user needs a PayPal account to check out.

Type “Mark” if you do want users to have a paypal account, or “Sole” if they can checkout without a Paypal account \(with credit card\).

**Landing Page**

You can select which page to show customers once they’re redirected to PayPal.

Type “Login” to direct customer to the login form for PayPal \(if you selected “Mark” above\). Or type “Billing” to show show customers a form where they can enter their credit card data and possibly sign up for a PayPal account \(if you selected “Sole” above\).

### MasterCard Internet Gateway Service \(MIGS\)

Set up of this service needs to be done through your bank. So far it has been tested with Bendigo Bank.

### Pin Payments

For Pin Payments you only require your API key. You need to set up an account with Pin Payments first, and can get a discount by signing up as an OFN member \([https://pin.net.au/partners/open-food-network/signup](https://pin.net.au/partners/open-food-network/signup)\)

**API Key:**Enter your “Live Secret API Key’ here – you can find this in your PinPayments account \(see below\). First from your account, select API Keys. Then once you have generated an API key, copy the ‘Live Secret API Key’ and paste it into the API key field in OFN.

![](https://openfoodnetwork.org/wp-content/uploads/2015/05/API-Keys.png "API Keys")

![](https://openfoodnetwork.org/wp-content/uploads/2015/05/API-2.png "API Key")

**Server:**Type ‘live’ – this is case sensitive.

## Fees on Payment Methods

[![](https://openfoodnetwork.org/wp-content/uploads/2015/05/Calculator.png "Calculator")](https://openfoodnetwork.org/wp-content/uploads/2015/05/Calculator.png)

You can attach a fee to payment methods. Most commonly this is used to pass on a payment fee to the customer, such as the Paypal charge. First you should select a fee calculator, then enter the value. A full description of the various fee calculators is below.

Note: Payment method fees do not include tax.

#### Fee Calculators

**Flat Percent **– This fee is charged as a percentage of the total amount charged in the order.

**Flat Rate \(per order\)**– This fee is applied as standard fee to all orders, regardless of the size of the order.

**Flexible Rate**– This calculator is typically used for promotional discounts where you charge a reduced fee as the customer makes more purchases of that item. This fee applies to items and products listed per kg or L.

* ‘First Item Cost’: The fee charged for the first item in the order.
* ‘Additional Item Cost’: The fee charged for aditional items beyond the first.
* ‘Max Items’: The maximum number of items on which the fee will be applied. Items purchased beyond this amount will be not be charged the fee.

For example: If the first cost is $2, Additional Item Cost is $1 and the maximum items is three. If a customer orders 5 of the item, they will be charged $2 for the first item, $1 for the second and third, and no fee for the fourth and fifth.

**Flat Rate \(per item\)**–  This fee is a constant fee, applied to products listed as ‘items’. \(it will not be applied to products listed as per kg, or per L\)

**Price Sack**– This fee is used to charge a discount on fees for orders which exceed a certain dollar amount.

* ‘Minimum Amount’: If the order’s total is below this amount, they will be charged the ‘Normal Amount’.
* ‘Discount Amount’: Orders which are equal to or greater than the minimum amount will be charged the ‘Discount Amount’.

_Have a suggestion for how we could improve this feature? Send us an email or join the conversation on our community forum._

