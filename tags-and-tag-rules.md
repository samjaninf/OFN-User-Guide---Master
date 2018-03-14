# Tags and Tag Rules

Using tags and tag rules allows you to customise the shopping experience for certain customers. Currently this includes:

* Making particular variants visible/invisible

* Making certain shipping methods visible/invisible

* Making certain payment methods visible/invisible

* Making order cycles visible/invisible

Most often this feature is required by enterprises who have different shop setups for members/non-members or different groups of customers such as wholesale/retail customers.

Using the tagging feature involves two main steps:

1. Applying a **tag **your customers
2. Setting up a **tag rule**

### Tagging Customers

Your [Customers ](/customer-accounts-and-tagging.md)page lists all customers who have placed an order in your shop, as well as any customers you have manually added to your customer list.

The first step to setting up a tag rule is to tag all of the customers who you want the rule to apply to.

For example, if I want to create a rule which makes free delivery available to wholesale customers only, you'll need to tag all of your wholesale customer with the same tag.

To create a tag, type the tag in the **tag** column next to a customer and hit the enter button when you’re done. The name of the tag is not important, so use something that makes sense to you \(your customers can't see your tags\). For this example you could use 'wholesale' or just 'ws'.

> Note: You must type the tag with identical characters each time - tags are case sensitive.

You can add multiple tags to a single customer \(e.g. you might have a rule for 'wholesale' customers, and a rule for 'priority' customers\).

[![](https://openfoodnetwork.org/wp-content/uploads/2015/10/Customer-taggs.png "Customer tags")](https://openfoodnetwork.org/wp-content/uploads/2015/10/Customer-taggs.png)Applying tags alone will have no effect until you create a **tag rule** relating to that tag.

#### Tags in reports

Some users apply tags to customers without setting up any tag rules. This is because it helps them with reporting.

Any tags that you apply to customers will also show up in your **Order cycle customer totals** [report](/reports.md), next to this customer’s order. If you export these reports as a CSV, in excel you can then filter your reports according to these tags, making it easy to sort your orders based on certain information.

## Tag Rules

Once you have tagged your customers you can define how certain feature will apply to customers with different tags. Currently you can use tags to change four elements:

* Making particular variants available/unavailable

* Making certain shipping methods available/unavailable

* Making certain payment methods available/unavailable
* Making order cycles visible/invisible

To set up your tags go to your Enterprise Settings and select **Tag Rules**.

### By Default

By default, all items will be visible to all customers whether they are tagged or not. The general approach is to then create a rule dictating that certain elements \(variant, shipping/payment methods or order cycles\) will be invisible to certain customers who are tagged. However, if you wish to change this default, such that tagged items are ‘not visible’ until a rule is setup reversing this, you can do so by changing your ‘By Default’ rules.

The example below shows that my shipping methods tagged ‘wholesale’ will now be invisible by default. If I then wish to make these shipping methods available to customers tagged wholesale I’ll need to set up a Tag Rule below overriding this default.

[![](https://openfoodnetwork.org/wp-content/uploads/2015/10/Default-tags.png "Default tags")](https://openfoodnetwork.org/wp-content/uploads/2015/10/Default-tags.png)

### Tag Rules

Keeping in mind your default setting above, you can now apply rules to vary the default settings for certain customers.

Firstly, you’ll need to select which tag your new tag rule will apply to. To do this type the tag into the ‘for customers tagged:’ field.

Next you can select which condition your rule is based on.

[![](https://openfoodnetwork.org/wp-content/uploads/2015/10/Rule-Typess.png "Rule Types")](https://openfoodnetwork.org/wp-content/uploads/2015/10/Rule-Typess.png)

##### **Show or Hide Variants in my shopfront**

This rule lets you make particular variants visible/invisible to tagged customers. For this rule to operate you need to have tagged the customer and the product variant **in your inventory** with the same tag. The screenshot below shows that my 10kg apple variant is tagged ‘wholesale’ in inventory.

[![](https://openfoodnetwork.org/wp-content/uploads/2015/10/Inventory-tagged.png "Inventory tagged")](https://openfoodnetwork.org/wp-content/uploads/2015/10/Inventory-tagged.png)

* **Invisible: ** If by default your variants are visible, you can select to make them invisible for customers with a particular tag.
* **Visible: ** If by default your variants are invisible, you can select to make them visible for customers with a particular tag.

The example below shows that my wholesale variants are invisible by default. A rule has been created so that variants tagged wholesale are made visible just for customers tagged ‘wholesale’.

[![](https://openfoodnetwork.org/wp-content/uploads/2015/10/Inventory-taggedd.png "Inventory tagged")](https://openfoodnetwork.org/wp-content/uploads/2015/10/Inventory-taggedd.png)

##### Show/Hide shipping methods

This rule lets you make particular shipping methods specifically available or unavailable to certain customers. For this rule to operate you need to have tagged the customer and the shipping method with the same tag. To tag a shipping method, go to **edit shipping method **and apply the relevant tag. E.g. the shipping method below has been tagged ‘wholesale’.

![](https://openfoodnetwork.org/wp-content/uploads/2015/10/Tagging-a-shipping-method.png "Tagging a shipping method")

* **Invisible:**
   If by default your shipping methods are visible, when you set the rule where ‘shipping methods tagged\_are invisible’ shipping methods with the tag will be hidden from customers with a matching tag when they checkout. Untagged shipping methods will still be visible to these customers.
* **Visible:**
  If by default your tagged shipping methods are invisible, you can make them visible to particular customer by setting a ‘shipping methods tagged\_are visible’ tag rule.  Customer without tags or with different tags will still be unable to see this shipping method at checkout.

##### **Show/Hide payment methods**

This rule lets you make particular payment methods specifically available or unavailable to particular customers. For this rule to operate you first need to have tagged the customer and the payment method with the same tag. To tag a shipping method, go to **edit payment method **and apply the relevant tag. E.g. the payment method below has been tagged ‘wholesale’.

[![](https://openfoodnetwork.org/wp-content/uploads/2015/10/Tagged-payment.png "Tagged payment method")](https://openfoodnetwork.org/wp-content/uploads/2015/10/Tagged-payment.png)

* **Invisible:**
   If by default your payment methods are visible, when you set the rule where ‘payment methods tagged\_are invisible’ payment methods with the tag will be hidden from customers with a matching tag when they checkout. Untagged payment methods will still be visible to these customers.
* **Visible:**
  If by default your tagged payment methods are invisible, you can make them visible to particular customer by setting a ‘payment methods tagged\_are visible’ tag rule.  Customer without tags or with different tags will still be unable to see this payment method at checkout.

##### Show/Hide order cycles at my shopfront

This rule lets you make certain order cycles visible to certain customers only. For this rule to operate you need to have tagged the customer and the order cycle with the same tag. To tag an order cycle, see the Tags tab in the outgoing section of an order cycle \(see below\).

> Note: This tag rule is only available to hub shops currently.

[![](https://openfoodnetwork.org/wp-content/uploads/2015/10/Outgoing.png "Tag OC in Outgoing")](https://openfoodnetwork.org/wp-content/uploads/2015/10/Outgoing.png)

* **Invisible:**
   If by default your order cycles are visible, when you set the rule where ‘Order cycles tagged\_are invisible’ order cycles with the tag will be hidden from customers with a matching tag. Untagged order cycles will still be visible to these customers.
* **Visible:**
  If by default your order cycles are invisible, you can make them visible to particular customer by setting a ‘order cycles tagged\_are visible’ tag rule.  Customer without tags or with different tags will not see this order cycle.



