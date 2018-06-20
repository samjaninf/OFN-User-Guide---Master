# Subscriptions- creating and managing orders

{% hint style="info" %}
This feature is LAUNCHING SOON
{% endhint %}

This page describes how shops can setup unique subscriptions for individual customers, including which items are in the subscription, which schedule the subscription applies to and pausing and editing the subscription.

> Before working your way through this page check out [Subscriptions - Configuration](https://github.com/ofn-user-guide/ofn-user-guide-master/tree/d5a1113e673b0e22198ca207b1db61339799868a/subscriptions/subscriptions%20-%20configuration.md) which covers how enterprise can activate the subscriptions feature, and setup groups of order cycles called Schedules, that the subscriptions will be applied to.

## Before you start…

Before you can create subscription orders for your customers there are a number of pre-requisite steps:

1. Have a shop enterprise with active [Shipping](../../basic-features/shipping-methods.md) and [Payment methods](../../basic-features/payment-methods.md)

Subscriptions can only be setup to use manual payment methods \(such as cash, or bank transfer\) or [Stripe](../../basic-features/payment-methods.md#payment-providers). Using Stripe is recommended, as this allows you to bill your customer's credit card automatically each time their subscription is processed.

1. Activate subscriptions for your shop - see [Subscriptions - Configuration](https://github.com/ofn-user-guide/ofn-user-guide-master/tree/d5a1113e673b0e22198ca207b1db61339799868a/subscriptions/subscriptions%20-%20configuration.md)
2. Setup at least one schedule of order cycles - see [Subscriptions - Configuration](https://github.com/ofn-user-guide/ofn-user-guide-master/tree/d5a1113e673b0e22198ca207b1db61339799868a/subscriptions/subscriptions%20-%20configuration.md)
3. Add any customers who will have subscriptions to your [Customer list](https://github.com/ofn-user-guide/ofn-user-guide-master/tree/d5a1113e673b0e22198ca207b1db61339799868a/customer-accounts-and-tagging.md).

Once you have configured the above, you’re ready to setup individual subscriptions for your customers.

{% hint style="info" %}
 In this first version of the subscriptions feature, shops must setup subscriptions on behalf of their customers. There is no customer facing place where customers can setup their own subscription.
{% endhint %}

## Create subscriptions

Click on **Orders** in the blue horizontal menu and then select **Subscriptions** in the green sub-menu.

Click **+ New Subscription** to setup a recurring order for your customer.

![](../../.gitbook/assets/new-subscription-basic-details.png)

**Customer:** 

Select a customer from the drop-down list.

\* You can only create a subscription for a customer who is on your [Customer List](https://openfoodnetwork.org/user-guide/advanced-features/customer-accounts-and-tagging/).

**Schedule:** Select the schedule, or order cycle group, that this customer wants to subscribe to.

{% hint style="info" %}
you must have created a schedule of order cycles before you can create a subscription. Instructions [here](subscriptions-configuration.md).
{% endhint %}

**Payment method:** Select the customer’s preferred payment method. This must be either Stripe or a manual payment method such as cash. Paypal and Pin Payments are not supported for subscriptions.

**Shipping method:** Select the customer’s preferred shipping method.

**Begins at:** This is the date that the customer’s subscription will start to be generated. If this date is midway through an open order cycle in their schedule there will be an order generated for that order cycle. If not the first order will apply to the next order cycle which open in their schedule.

**Ends at:** After this date the customer’s standing orders will no longer be generated. This field is optional, if left blank the will continue to be generate indefinitely. 

How precisely does the end date interact with the OC dates? If the customer's subscription end date is after the opening date of an OC in their schedule, but before the end date of the OC, there won't be an order generated. The order will only be generated if the customer's end date, is after the OCs close date.

#### Address

Fill out the customer’s billing and shipping details. If there is saved customer shipping and billing details in your customers page, this information will load automatically.

![](../../.gitbook/assets/new-subscription-address.png)

Add Products

\(?\) clarification about which products an enterprise can add to SOs.

\(?\) clarification about what happens if the price of an item changes.

![](../../.gitbook/assets/new-subscription-add-products.bin)

#### Summary

Check that details are correct and then click Create Subscription or Cancel.

## Edit a customer’s subscription

### Edit the base subscription

From the **Subscriptions** page, click on the **edit** button next to the subscription you want to edit.

![](../../.gitbook/assets/edit-subscription.bin)

From here you can edit which products are in the subscription, the preferred shipping and payment methods, the starting and ending dates and the customer’s details.

{% hint style="info" %}
 You cannot change a subscription’s schedule. Instead the subscription must be recreated in the new preferred schedule.
{% endhint %}

Does changing customer details in Customer page update them in SO? \(?\)

### Edit one specific order

If you want to change a single upcoming order in a subscription you can click on the number in the customers’ orders column.

This will reveal all upcoming orders in the schedule, and you can then edit a specific order.

![](../../.gitbook/assets/edit-single-subscription-order.bin)

### Pause a subscription

From the subscriptions page, click on the **pause** button next to the subscriptions you wish to pause. This will prevent all future orders in the subscription from being generated, until it is activated again. To un-pause a subscriptions, click on the play button.

{% hint style="info" %}
 If you pause a subscription while an order cycle is still open, you'll be asked whether you'd like to keep the current order or not. If you un-pause a subscription while an OC is open an order will be generated for this customer if they're subscribed to that schedule.
{% endhint %}

![](../../.gitbook/assets/pause-subscription.bin)

### Delete a subscription

From the **subscription** page, click the **cross** button next to the subscription you wish to delete. This will prevent any future subscriptions from being generated and delete this subscription permanently.

![Delete standing order](https://openfoodnetwork.org/wp-content/uploads/2017/03/Delete-standing-order.png)

{% hint style="info" %}
 If you delete a subscription while there is an open order cycle you'll be asked whether you want to keep the customer's open order, or if they want to delete the current order.
{% endhint %}

