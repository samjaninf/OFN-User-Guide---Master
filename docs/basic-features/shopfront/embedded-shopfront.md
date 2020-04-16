# Embedded Shopfront

This feature lets users who have Harvest To Order shopfronts embed their shop into their own website. Customers get a more fluid experience, avoiding the need to be redirected between your main website \(which may have information about your enterprise\) and the shop front. It also allows enterprise to retain some of their visual branding in their Harvest To Order shop.   
When you embed your Harvest To Order shop in your own site, your Harvest To Order based shop will remain, so customers can choose where they want to shop. 

{% hint style="danger" %}
**This feature will soon be completely redesigned**.   
  
It is currently based on the same technology which allows to you embed a YouTube video \(or other\) into your website.

There are the following limitations of this 'iframe' approach:

* if you have a lot of products in your shop, browsing from your website in the shop will be very slow
* if your buyers connect from an ipad / iphone, they will not see the entire list of products because the store is not "scrollable" from these terminals.

We hope to replace this embedded shop front feature with a new 'plugin'-based version.

_**Until the update is complete we don't recommend use of embedded shop fronts.**_
{% endhint %}

## Requirements

### Platforms

This feature works \(with the limitations above\) on any kind of website hosting platform which allows you to add custom html to the page where you want to embed the shop. WordPress, Squarespace, Wix , for example, all permit this.

### Security

Because Harvest To Order is an eCommerce platform, and handles monetary transactions, it has a higher security requirement than text only websites. Therefore, you’ll need to setup SSL/TLS on the website you want to embed your Harvest To Order shop into if you haven’t already.

You can get such a security certificate for free from [Let’s Encrypt](https://letsencrypt.org/) or for around $10-$30 for a paid service.

### Harvest To Order Shop

Of course, the last requirement is that you have a shop setup on Harvest To Order. You’ll need to know your shop’s Harvest To Order URL in the setup steps below.

## Getting setup

### **Contact your local Harvest To Order team**

First of all, you’ll need to [contact your local Harvest To Order team](https://harvesttoorder.com/contact/) and let them know that you want to embed your Harvest To Order shop in your own website. You’ll need to provide them with your external domain. E.g. happyhenfarm.com.au so they can grant permission for your website to communicate with Harvest To Order.

### **Adding Custom HTML to your website**

Embedding your shop is as simple as inserting a line of code into your website. This is the line of html that you should insert into the page where you want the shop:

```text
<iframe src=" https://harvesttoorder.com/happy-hens-farm/shop?embedded_shopfront=true"style="width:100%;min-height:35em"></iframe>
```

In the html above make sure to replace ‘happy-hens-farm’ with your shop’s unique Harvest To Order [permalink](../enterprise-profile/enterprise-settings.md#primary-details) \(found in your Enterprise Settings -&gt; Primary Details\).

Once you’ve done this, you should see your Harvest To Order shopfront appear on your webpage.

### **Styling**

Depending on the styling of your website you may need to add some CSS tweaks. They may be needed to avoid having two scroll bars, and to make sure the length and width of the embedded shop looks visually appealing. 

{% hint style="info" %}
Make sure to test the display of your embedded shop on a mobile device.
{% endhint %}

If the mobile display is misbehaving you may need further CSS tweaks. The tweaks required will be different for every website.

### **Example**

We have setup an [example of an embedded shop](https://harvesttoorder.com/user-guide/advanced-features/demo-embedded-shop/) for you to look at and play with.

## Instructions for Customers

{% hint style="info" %}
Customer will need to accept cookies on your website in order for them to view the embedded shop front.  This is a necessary part of the Shop integration.
{% endhint %}

