# Reports

Access reports by clicking on **Reports** in the horizontal heading.

![](../.gitbook/assets/access-reports.png)

This will take you to a table listing all of the reports available.

![](../.gitbook/assets/reports-table.png)

The two most useful and commonly used reports are the **Order Cycle Supplier Totals** and the **Order Cycle Customer Totals**. If you plan to fulfill orders on a indivdual basis, the Order Cycle Customer Totals report will be most relevant to you. If you intend to fulfill orders in batches corresponding to an order cycle routine, the Order Cycle Supplier Totals will also be useful. The **Mailing List** and **Addresses** reports are also helpful for managing your customer’s details. The **Sales Tax** report is useful for enterprises dealing with GST reporting. Finally, the **Bulk Co-op** report helps with bulk ordering decision making.

## Order Cycle Customer Totals

The picture below shows the information contained in an Order Cycle Customer Totals report. This report can be generated to reflect a particular order cycle by selecting an order cycle from the dropdown menu. As you can see, you may also select to download a CSV copy of this report \(an excel file\). The report shows each customers order, including thier email and contact details, the **product** they ordered, the **amount,**the **item \($\)** and the TOTAL. Lastly it also shows the shipping method they have selected. If you are fulfilling orders on an individual basis, this report gives you all the information to pack the order, contact the customer and arrange for delviery or collection. If you are preparing orders in bulk at the closing of an order cycle, this report can be used to guide your packing and delivery.

![Order Cycles Customer Totals Report](../.gitbook/assets/order-cycle-customer-totals.png)

## Order Cycle Supplier Totals

The picture below shows the information contained in an Order Cycle Supplier Totals report. Like the above report, this report can also be generated to reflect a particular order cycle by selecting an order cycle from the dropdown menu. As you can see, you may also select to download a CSV copy of this report \(an excel file\). In the report, the supplier is listed on the left. Next is listed all of the **products** and their **variants**, and the **amount** of each that sold. At the closing of an order cycle, this report clearly shows you how much of each product you will need on hand to successfully pack and fulfill all of the orders placed.

![Order Cycles Supplier Total Report](../.gitbook/assets/order-cycle-supplier-totals.png)

## Mailing List

The mailing list report shows the names and email addresses of customers who have placed orders in your store. You can filter the report according to order cycle, allowing you to alert customers if there are stock outs or changes to the delivery shedule. See below for an example. As with all reports, the list can be downloaded as a CSV file.

![Mailing List Report](../.gitbook/assets/mailing-list.png)

## Addresses

The Addresses report details your customer’s names, addresses, emails, phone numbers and the hub, or store, they shopped with. Again, this report can be filtered by order cycle.

![Addresses Report](../.gitbook/assets/addresses.png)

## All Products and Inventory \(on hand\)

The All Products and Inventory \(on hand\) reports can be used as a paper copy ordering sheet, for any customers who prefer to order on paper. It lists all of your products and their prices \(see below\). The **All Products** report lists all of your products regardless of whether they have on hand quantities above 0. The **Inventory \(on hand\)** report shows only products which have a positive on hand value.

![All Products Report](../.gitbook/assets/all-products.png)

## Enterprise Fee Summary

Enterprises can set up [enterprise fees](enterprise-fees.md) to identify and control allocation of costs / prices for different purposes. These fees enable price transparency and are revealed to customers in the shop. The Enterprise Fee Summary report is used to summarise how much of which fees were charged to whom. 

The report contains standard filtering by Hub, Producer and Order Cycle, as well as fields enabling selection of the Fee Names you want included, or which Shipping or Payment methods.

![](../.gitbook/assets/image%20%2823%29.png)

Example 1: a Shop includes a 2% fundraising fee on every order to donate, they can use this report to easily find the total funds raised within a particular order cycle. 

Example 2: a Hub pays a transport fee to a Producer that picks up produce from other farmers and brings it into the Hub. This fee is calculated on every incoming product into an order cycle. They use this report to work out how much to pay that Producer

Example 3: a Hub sets up a fee to show the amount they pay to Open Food Network to their customers \(see image below\).

![](../.gitbook/assets/image%20%282%29.png)

## Packing Reports

Some enterprises use their order confirmation emails as packing sheets, and others will create their own by modifying the Order Cycle Customer Totals report \(above\) to suit their desired format. These packing reports offer two additional options for packing slips.

**Pack by Customer** 

This report lists each customer who placed an order. It included each item ordered by the customers, along with the quantity ordered. It’s useful for shops who pack orders customer by customer.

**Pack by supplier**

This report lists each supplier and their products. Next to each product is the name of the customers who ordered this product, and the quantity they ordered. This report is useful for shops who pack orders according to supplier.

## Sales Tax

This report is useful to separate the tax component of sales, delivery and fees.

![Sales Tax Report](../.gitbook/assets/sales-tax-report.png)

## Xero Invoices

This report creates CSV files which can be imported into the accounting package ‘Xero’ to generate invoices for customers.

### Generating the report

![Xero Report Fields](../.gitbook/assets/xero-report.png)

**Date range:** You can filter orders by the date placed.

**Report type:**You can select to download a ‘detailed’ report, which includes a line item for each item the customer purchased, including any fees and adjustments to their order.

**Hub and order cycle:** As with all reports, the data can be filtered by the Hub when orders were placed and the order cycle they were in.

**Initial invoice number:** You want these new invoices to be numbered according to where you Xero invoice numbering system is at. So check in invoice what the last invoice number was and then type the next number into this field. This will mean that subsequent invoices will be numbered from this point.

**Invoice date:** You can select the date that you want the invoices to be marked with in Xero. This is editable once you have the invoice in Xero, but doing it here allows you to date multiple invoices at once.

**Due date:** You can select the due date to be marked on the Xero invoices. Again this is editable in Xero.

**Account code:** If you place a Xero account code here, all items in the invoice will be assigned to this account. This it aditable in Xero.

**Download as CSV:** When you are ready to download the file for import click this box and hit the **search** button.

### Importing the report into Xero

In Xero go to **Accounts**, **Sales** and click Import.

![Xero Import](../.gitbook/assets/xero-import.png)

Next you will select your downloaded OFN Xero report for upload. The settings you should select are shown below.

![Xero Import Steps](../.gitbook/assets/xero-import-steps.png)

Ignoring the address details will ensure your Xero customer data is unaltered. Selecting**Tax Exclusive**will ensure that products you have set to include tax in the OFN will include tax, but your tax free items will remain tax free.

## Bulk Co-op  Totals By Suppliers Report

This report tells shop managers whether they have reached their bulk ordering threshold, and by how much they have exceeded or fallen short of this amount. Note you need to setup bulk sizes for your products before using this feature, see the [Group Buy](https://openfoodnetwork.org/user-guide/advanced-features/group-buy/)advanced feature for instructions.

When their order cycle closes, this report can help the shop to answer the following questions:

* Did customers order enough of this product to justify ordering the bulk size from the supplier?
* If the [Group Buy](../advanced-features/products/group-buy-for-bulk-ordering.md) tool is enabled, how much extra product are my customers willing to purchase to help the group reach the bulk size threshold?
* How many bulk sizes should the shop order to meet the customer demand?
* If the shop orders the bulk size, how much stock will be left over? Or alternatively, how many customers will be disappointed if this product isn’t ordered?

See the example below for an illustration of how this report can be used:

This is an example of where the bulk ordering quantity has been reached:

![Radishes](../.gitbook/assets/radishess.png)

This is an example where the bulk order quantity has not been reached:

![Bok Choy](../.gitbook/assets/bok-choy.png)

* _Note the ‘Bulk Co-op Allocations’ report is similar in function to this report, but shows each customer’s order individually, rather than the cumulative total across all customers._

