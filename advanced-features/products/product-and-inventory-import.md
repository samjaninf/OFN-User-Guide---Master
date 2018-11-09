# Product and inventory import

{% hint style="info" %}
THIS FEATURE IS COMING SOON
{% endhint %}

The product and inventory import tool lets you upload a csv file to add and update your stock.

The product and inventory import tool can be found by clicking **Products** in the horizontal blue menu, and **product import** in the green menu.

Product import can be used in relation to [products ](../../basic-features/products.md)and [inventory](inventory-tool.md). There's four ways you can use the tool:

1. Import new products
2. Update existing product details
3. Import new inventory
4. Update existing inventory details

In all cases the process involves downloading a csv template, filling in the fields and then uploading your csv file back into OFN.

#### Product fields that aren't encompassed by the import tool

In the first version of this tool there are a few fields that aren't captured. Unfortunately in the mean time these fields will need to be setup or updated manually. See [product](../../basic-features/products.md) for details. 

* Image
* Properties \(All uploaded products will inherit the properties of the producer profile\).
* Product description
* Group buy settings

{% hint style="info" %}
If you need this functionality, please let [your local OFN](https://openfoodnetwork.org/ofn-local/) know. We welcome your feedback.
{% endhint %}

## 1\) Import New Products

Use these instructions if you want to add new products to a producer's profile.

{% hint style="info" %}
You can simultaneously upload new products and update existing products with a single CSV upload. The instructions in this guide are separated for clarity but you can combine new products and updates in the same spreadsheet.
{% endhint %}

### Prepare the CSV file for import

Firstly, download the **Product List Template CSV** file from the **Product Import** page and open it with excel \(or equivalent. [Google Sheets](https://www.google.com.au/sheets/about/) is a free option\)

You'll see that the template gives all the column headings required to successfully import a product. Each row is for a new product or variant. Below is a description of how to fill in each column.

![](../../.gitbook/assets/image.png)

{% hint style="info" %}
Note that all fields are case sensitive. E.g. you must use mL not ml , or Dairy not dairy.
{% endhint %}

| Column Title | Required? | Description | Example |
| :--- | :--- | :--- | :--- |
| producer | Y | This is the name of the producer profile that this product will be assigned to | Four Mile Farm |
| sku | N | The SKU code for this product | AD001265 |
| name | Y | This is the name of the product | Yoghurt |
| display name | N | This field applies if you are creating variants \(see instructions below\). If you're not creating a variant leave this field blank. | Rasberry Yoghurt |
| category | Y | Which category does this product sit in? The categories available are listed on the Product Import page | Dairy |
| units | Y | The weight, volume or quantity value | 500 |
| unit\_type | Maybe | What unit is it sold in \(g, kg, T, mL, L\)? If sold as an item \(e.g. bunch\) leave blank | g |
| variant\_unit\_name | Maybe | If the product is sold as an item \(e.g loaf, bunch, pumpkin\) write the item type here | Bunch |
| price | Y | The price of the product. If the item carries tax, this must be the tax inclusive price. | 3.70 |
| on\_hand | Maybe | If you have limited stock for the product type the stock level here. If you have infinite stock available \(you can always source it\) enter 0 and use the on\_demand column | 40 |
| available\_on | N | Leave blank |  |
| on\_demand | Maybe | If you have infinite stock available for this product, type 1, if you're using on\_hand leave blank. If you enter a number in on\_hand _and_ 1 in on\_demand, the product will be on demand. | 1 |
| shipping\_category | N | Leave blank |  |
| tax\_category | Y | If the price of your product includes tax type GST, if not leave blank | GST |

#### How to import variants

[Variants ](product-variants.md)are similar products that differ on size or flavour. By uploading them as variants rather than individual products, your shop will be less cluttered and easier for the customer to navigate. 

In the import process, variants are distinguished by the units \(such as salad sold in 2 size variants\) or display\_name fields \(such as a yoghurt sold in multiple flavours\) and grouped by product name.  As long as the product name is the same, the rows will be imported as variants

The example below shows a salad that comes in 500g and 750g variants, and a yoghurt that comes in multiple flavours.

| name | display\_name | price | units | unit\_type |
| :--- | :--- | :--- | :--- | :--- |
| Salad Bag |  | 3.50 | 500 | g |
| Salad Bag |  | 5.50 | 750 | g |
| Yoghurt | Banana | 4 | 500 | g |
| Yoghurt | Strawberry | 4 | 500 | g |

The image below shows how these products will display in the shop. Note that the 'name' field becomes the primary heading, and the 'display\_name' field becomes the secondary heading. In the case of the Salad Bag, the 'display\_name' field is blank, so the 'name' is used by default.

![](../../.gitbook/assets/image%20%281%29.png)

#### Unit type examples

Below are some examples to show how products with different units \(g, ml, kg and items\) should be uploaded.

| producer | **name** | **category** | **price** | **units** | **unit\_type** | **variant\_unit\_name** |
| :--- | :--- | :--- | :--- | :--- | :---: | :---: |
| Sue's Salads | Salad Bag | Vegetables | 3.50 | 500 | g |   |
| Henry Orchards | Fruit Juice | Drinks | 3.50 | 300 | ml |   |
| Fernwell Produce | Potatoes | Vegetables | 9.50 | 5 | kg |   |
| Tom's Bakery | Wholemeal Bread | Baked goods | 3.00 | 1 |   | loaf |

### Import the CSV

Once you have filled out the **Product List Template CSV** you are ready to upload it into OFN.

Go to **Products** &gt;  **Product Import.**

**Select import type:** Select Product List

**Select a spreadsheet to upload:** Find the csv file you wish to upload.

Because you are uploading new products, you can leave the '_Set stock to zero for all exiting products not present in the file_' checkbox unticked. 

Click **Upload**.

You'll be shown a summary of your upload, including any errors. You'll also be told how many products you are creating and how many you are updating. If you're happy with the upload results, click **save**. You can then upload another spreadsheet or go to the products page to view your new products.

{% hint style="info" %}
It's good practice to check that the products uploaded/updated as you intended.
{% endhint %}

## 2\) Update Existing Product Details

The instructions below relate to updating the details of an existing product. This tool is intended as a quick way to update product prices and stock levels.

{% hint style="info" %}
You can simultaneously upload new products and update existing products with a single CSV upload. The instructions in this guide are separated for clarity but you can combine new products and updates in the same spreadsheet.
{% endhint %}

### Prepare the CSV file for import

The process for updating product details is similar to uploading new products. The first step is to download the **Product List Template** and fill in the product names and the supplier names. If you have this spreadsheet on hand from a previous upload even better. 

The system requires seven fields, which it uses to identify the correct product you want to update. There are four fields which can be updated. Three fields cannot be updated with the import tool.

| Required fields \(you can't update\) | Fields you can update | Fields that won't update and aren't required |
| :--- | :--- | :--- |
| \*supplier | sku | ^variant\_unit\_name |
| \*name | price | ^tax\_category |
| ^category | on\_hand | ^shipping\_category |
| \*units | on\_demand |  |
| ^unit\_type \(if applicable\) |  |  |
| ^variant\_unit\_name \(if applicable\) |  |  |
| \*display\_name |  |  |

_^ if you try to update these fields you'll see an error message_

_\*If you try to update these fields you'll actually create new products or variants, rather than update an existing product._

The green columns are required, the orange are able to be updated, the white cannot be updated and aren't required.

![](../../.gitbook/assets/image%20%2813%29.png)

### **Import the CSV**

Once you have filled out the **Product List Template CSV** you are ready to upload it into OFN.

Go to **Products** &gt;  **Product Import.**

**Select import type:** Select Product List

**Select a spreadsheet to upload:** Find the csv file you wish to upload.

**Set stock to zero for all exiting products not present in the file:** If you select this tickbox the system will set the 'On Hand' value to zero for all products already your product list. If a product was 'On Demand' it will remain 'On Demand. The Products in this import will retain the stock level you have set in the csv.

Click **Upload**.

You'll be shown a summary of your upload, including any errors. You'll also be told how many products you are creating and how many you are updating. If you only intended to update products but you see that a product is being created, you can see which row it is and go back and fix your spreadsheet. If you're happy with the upload results, click **save**. You can then upload another spreadsheet or go to the products page to view your new products.

## Import New Inventory

Coming soon

## Update Existing Inventory Details

Coming soon

