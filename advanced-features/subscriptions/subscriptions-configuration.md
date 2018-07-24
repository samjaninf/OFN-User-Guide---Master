# Subscriptions - configuration

## 1\) Enable subscriptions

{% hint style="info" %}
While subscriptions is in Beta mode, you'll need to contact [your local OFN](https://openfoodnetwork.org/ofn-local/) representative to have subscriptions activated for your shop.
{% endhint %}

To enable the Subscription tool, you’ll need to activate the feature in your enterprise’s settings. Once turned on, the additional subscription tabs and controls will become visible to you. These settings can be found in Manage your enterprise, in the [**Shop Preferences**](../../basic-features/enterprise-settings.md#shop-preferences) ****tab.

**Subscriptions**: To activate subscriptions, select Enable.

**Guest orders**: We recommend that shops offering subscriptions also require customers to login before they can shop with you. This will ensure that any customer with a subscription will login and see their existing subscription order, and not accidentally place a duplicate order.

**Change orders**: Enterprises can choose whether or not customers are allowed to edit their order while the order cycle is open. 

* If you allow customers to change their order, they can remove items from their subscription order or cancel the order. If customers want to add something to their order they will need to place a new order.
* If you don't allow customer to change their order, they'll need to contact you if they wish to remove items from their order, or cancel it. With this setting, customers can still chose to place another order.

## 2\) Make sure you have Shipping and Payment methods setup

When you get to the stage of creating the customer's subscription, you'll need to select which shipping method they'll use and which payment method they'll be billed with.

#### **Shipping methods**

You can apply any shipping or payment method to a subscription. See here for [instructions for setting up shipping methods](../../basic-features/shipping-methods.md).

#### **Payment methods**

You can only assign two types of payment methods to subscriptions. See here for [instructions for setting up payment methods](../../basic-features/payment-methods.md).

**1\) Manual payment methods**: This includes cash, or bank transfer. 

**2\) Stripe:** Stripe is a payment gateway which takes payment with credit cards. When you apply a Stripe payment method to a customer's subscription, Stripe will bill their credit card automatically each time one of their subscription orders is processed. The amount they are charged will reflect any changes they've made to the subscription order, and they will not be changed if you cancel or pause their subscription.

Before a shop can successfully charge the customer, the customer must signup with OFN, save a default credit card in their account _and_ grant permission to your shop to charge the credit card. Further detail about these steps are on the [subscriptions - the customer perspective](subscriptions-the-customers-perspective.md) page.

Note, when you setup Stripe to be used in subscriptions it's a good to make the payment method name and description clear. 

For example, rather than calling the payment method 'Credit card' you might like to call it 'automated credit card billing for subscriptions'. A possible description could be 'Your default credit card saved in your OFN account will be charged when your subscription order is confirmed on Wednesday nights'. This name and description will show on the email confirmation to subscription customers \(see example below\), so it's good to make it details so the customer knows what to expect.

![](../../.gitbook/assets/image%20%288%29.png)

## 3\) Gather information from your customers

To setup a subscription for a customer you'll need to get some information from them, as detailed below. You may do this via email or a [google form](https://www.google.com.au/forms/about/). 

**Name**, **phone number** and preferred **email address**. As discussed next, you must add your subscription customers' emails to your [Customer List](../shop-setup/customers.md) before you can create a subscription for them, and you'll need this info.

**Billing and shipping address**: You'll need this information when you setup their subscription.

**Products:** Which items to they want to include in their subscription. You'll need this information when you setup their subscription.

**Shipping method**: You need to assign their subscription order to a shipping method.

**Payment method**: Customers can select from your manual payment methods \(e.g. cash, bank transfer\), or paying with their credit card through your shop's stripe account. In the case that you are offering automated direct debiting to credit cards using stripe, you will need your customers to add their credit card information into their OFN account \(see below\).

**Dates** they want their subscription to span: Remember, for a subscription order to be created for a given order cycle it must have a start date either before or after the order cycle opening date, and the subscription end date must be after the OC close date.

## 4\) Add your subscribers to your customer list

Before you can setup a subscription order for a customer they need to be added to your Customers list. See here for instructions for maintaining your [Customers list](../shop-setup/customers.md).

**After you've added your customers to your customer list email them** and ask them to sign up for an account on OFN. Instructions for doing this can be found [here](subscriptions-the-customers-perspective.md#signing-up-to-ofn). If you plan to bill customers using Stripe, you need to also request that they [save their credit card details and authorise your shop to charge their card](subscriptions-the-customers-perspective.md#saving-credit-cards-and-authourising-charges).

You can add customers to your Customer list before or after they've signed up for an account with OFN. However, note that before a subscription order can be successfully setup the customer must signup with OFN and confirm their email.

Also, if you want to use Stripe to take credit card payment from subscribers, you must add them to your customer list before they can grant your shop permission to bill their credit card.

Thus we suggest the following process: a\) contact your customers to get their required information b\) add them to your customer list c\) email them and ask them to signup to OFN \(and grant you permission to bill their card, if your shop will use Stripe\) and then d\) [you create their subscription](subscriptions-creating-and-managing-orders.md#6-create-subscriptions).

## 5\) Schedules

{% hint style="info" %}
If you are new to OFN we encourage you to get familiar with setting up [order cycles](../order-cycles/) before setting up schedules.
{% endhint %}

### About Schedules

Subscriptions are setup so that every time a shop opens an order cycle, orders are automatically generated for customers who have a subscription with that shop. However, the system has the added flexibility of allowing shops to decide _which_ order cycles the subscription will apply in. This allows shops to have some order cycles which trigger subscription orders to be created, and some which do not.

Which order cycles trigger subscriptions is controlled through an additional element in the Order Cycle setup process, called ‘schedules’. Schedules are groups that order cycle can be assigned to. Once a schedule has been created, customer subscriptions are applied to the schedule, so that an order for their subscription will only be generated for new order cycles in that schedule.

Let’s clarify with some examples:

**Example 1**

Harvest Hub runs weekly order cycles. Customers are able to subscribe to either a weekly, or fortnightly order.

In this case there will be two schedules. One that contains all order cycles- the weekly subscribers will have their subscription assigned to this schedule. The second schedule will contain only every second order cycle- the fortnightly subscribers will have their subscription assigned to this schedule.

#### Example 2

Delta Farm runs two order cycle a week, one for a Monday delivery and one for a Thursday delivery.

Most of their customers subscribe to one delivery a week, but some of their hospitality customers subscribe to both the Monday and Thursday delivery.

In this case there will be two schedules, one for the Monday customers and one for the Thursday customers. Those customers who want a subscription on both days can have a subscription applied to both schedules.

### Create a schedule

Once you have[ enabled the subscription feature](subscriptions-configuration.md#1-enable-subscriptions), you will see the Schedule functionality in the order cycle interface. To create a schedule click on the **+ New Schedule** button.

![](https://openfoodnetwork.org/wp-content/uploads/2017/02/New-order-cycle.png)

Note: You must have at least one order cycle that can be added to the schedule before you create it.

![](../../.gitbook/assets/new-schedule.bin)

**Name:** Give the schedule a logical name which describes this group of order cycles. E.g. ‘weekly’, ‘monthly’, ‘Tuesday Deliveries’, ‘wholesale’ or ‘retail’. This name is only visible to you in the backend, not to customers.

You can add existing order cycles into and out of the new schedule by clicking the &lt; and &gt; buttons.

Click **create** when you are finished.

### Edit or Delete a schedule

To edit or delete a schedule, click on the schedule’s name next to a corresponding order cycle, in the ‘schedules’ column.

Note: This column may need to be made visible in the columns setting dropdown.

![](../../.gitbook/assets/show-schedules.bin)

You can change the name of the schedule, add/remove order cycles from it or delete the schedule.

![](../../.gitbook/assets/delete-schedule.bin)

> Note: You cannot delete a schedule if there are subscriptions associated with it.

### Adding or removing order cycles from schedules

You can add and remove order cycles from schedules by either editing the schedule \(above\), or by editing the order cycle and adding/removing the schedule in the ‘schedules’ field \(below\).

![](../../.gitbook/assets/oc-schedule.bin)

Order cycles may be in more than one schedule. For instance, in the Harvest Hub example above, every second order cycle will be in both the weekly schedule and the fortnightly schedule.

