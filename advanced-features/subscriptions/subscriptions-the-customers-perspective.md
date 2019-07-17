# Subscriptions - the customer's perspective

This page details what a customer with a subscription can expect. It also highlights some things that shops offering subscriptions should be aware of.

## Signing up to OFN

Customers need to have an account with OFN before you can process subscription orders for them.

To sign up customers can go to [https://openfoodnetwork.org.au/login](https://openfoodnetwork.org.au/login)

They'll just need their email address, and to create a password. 

After signing up they'll be sent a confirmation email. Once they click on this link that will confirm their new account, and they can then login.

## Saving credit cards and authourising charges

Customer who want to pay for their subscription orders via automated charges onto their credit card need to a\) save their preferred card in their OFN account and b\) grant the shop permission to charge that card. Only after they have done this will the shop be able to setup a subscription which charges their credit card.

### a\) Saving credit card details in the customer account

The Customer Account page can be accessed at [https://openfoodnetwork.org.au/account\#/cards](https://openfoodnetwork.org.au/account#/cards) . 

Your customer can save one or more cards in their account, in the **credit cards** tab.

![](../../.gitbook/assets/image%20%2825%29.png)

The card which is denoted as 'default' will be charged automatically by Stripe if they have a subscription with Stripe as the chosen payment method. If none is selected as 'default' their credit card payments won't be processed.

If your customer saves credit cards in their account, they'll also be able to quickly select these when they shop in your shop at checkout.

![](../../.gitbook/assets/image%20%284%29.png)

### **b\) Authourising a shop to charge their default card**

As well as saving a card in their account the customer needs to authorise your shop to charge their default card.

**You should add your customers to your** [**Customer List**](../shop-setup/customers.md) **before you ask them to save their credit card details and authorise your shop to bill their card.** If you've added a customer to your customer list, when that customer creates an account with OFN and logs in to save their card, they _will_ see your shop and be able to grant it with permission to bill their card \(e.g. below\). 

![](../../.gitbook/assets/image%20%2831%29.png)

If you haven't added them to your customer list by the time they go to save their card they _won't_ see your shop to grant the required permission \(e.g. below\). If this happens, you'll need to add them to your customer list, and then they'll need to log back in to grant the authorisation. 

![](../../.gitbook/assets/image%20%2817%29.png)

Below is an example of a customer who has granted permission for a Farm shop to charge them.

![](../../.gitbook/assets/image%20%2818%29.png)

## Email notifications

The subscriptions feature includes a number of automatically generated emails which are sent to customers each time one of their subscription orders is processed.

#### Email 1 - When the Order Cycle opens

The first email is triggered the moment an order cycle in the customer's subscribed schedule opens. This email lets the customer know that their subscription order has been opened. The customer can see which items are in the order and the amount they'll be charged. The email also contains their shipping and payment information.

![](../../.gitbook/assets/image%20%285%29.png)

#### Modifying the order

Whether or not a customer can make changes to their subscription order will depend on the shop's settings in [Shop Preferences](../../basic-features/enterprise-settings.md#shop-preferences).

If the shop **does not all customers to change their orders,** their email will be the same as above. If they wish to cancel their order, or make changes, they'll need to contact the shop to request the changes.

If the shop **allows customers to change their orders**, the text in the blue text box will be slightly different to the email above and there will be a link which will take customers to their order \(see below\). Currently customers will only be able to remove items from their order, or change the quantities of existing items. If they want to add a new item to their order they'll need to either place a new order or contact the shop and ask them to make this change for them.

![](../../.gitbook/assets/image%20%2813%29.png)

#### Products unavailable

In the case that a product in the customer's subscription was not available, due to limited stock or the product not being in the Order Cycle, they'll be alerted in the first email \(example below\).

![](../../.gitbook/assets/image%20%2821%29.png)

#### Email 2 - When the Order Cycle closes

The final email goes to the customer when the order cycle closes. This email confirms the final order, including any adjustments they made. 

![](../../.gitbook/assets/image%20%2812%29.png)

#### Unable to charge credit card

At the close of the order cycle, charges to credit cards will be initiated for customers who chose to be charged by Stripe. If there are any issues with the billing of their card they'll be alerted in the second email. Note in the case of a unsuccessful charge to the card, the order is still confirmed, it's just left in the 'balance due' state.

Possible reasons for an unsuccessful charge:

* Insufficient funds
* Card expired
* The customer has revoked permission for the shop to charge their card
* The customer has removed the 'default' status of their credit card

The shop will also be alerted of any unsuccessful charges.

## Frequently asked questions from customers

#### How can I pause my subscription?

If you need to pause your subscription you'll need to contact the shop and ask them to pause it. Be sure to let them know when you want to resume your subscription.

#### Will the price of my subscription remain the same, even if prices change in the shop?

No, if product prices change after you setup your subscription order, you wil be charged according to the updated prices.

#### How can I cancel my whole subscription?

If a customer wants to stop their subscription, they'll need to contact the shop manager and let them know. Only the shop manager can delete a subscription.

#### How can I cancel a single order of my subscription?

If a customer wants to cancel a single subscription order, there are two ways to do this depending on the shop's settings. 

If the shop __**does not** allow customers to make changes to their orders, the customer will need to contact the shop and let them know which order to cancel. 

If the shop **does** allow customer to make changes to their orders, the customer can wait until they receive the first confirmation email \(when the OC opens\) and from there they can edit their order and cancel it.

