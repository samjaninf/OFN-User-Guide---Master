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

## 1\) Import New Products

Use these instructions if you want to add new products to a producer's profile.

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

[Variants ](product-variants.md)are similar products that differ on size of flavour. By uploading them as variants rather than idividual products, your shop will be less cluttered and easier for the customer to navigate. 

Iin the import process, variants are distinguished by the units \(such as salad sold in 2 size variants\) or display\_name fields \(such as a yoghurt sold in multiple flavours\) and grouped by product name.  As long as the product name is the same, the rows will be imported as variants

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

Go to Product Import 

## 2\) Update Existing Product Details

The instructions below relate to updating the details of an existing product. 

This tool is intended as a quick way to update product prices and stock levels.

The process for updating product details is similar to uploading new products. The first step is to download the **Product List Template** and fill in the product names and the supplier names. If you have this spreadsheet on hand from a previous upload even better. 

The system requires six fields, which it uses to identify the correct product you want to update. There are also 6 fields which can be updated. Some fields cannot be updated with the upload tool.

| Required fields \(you can't update\) | Fields you can update | Fields that won't update and aren't required |
| :--- | :--- | :--- |
| supplier | sku | variant\_unit\_name |
| name | display\_name | tax\_category |
| category | price | shipping\_category |
| units | on\_hand |  |
| unit\_type \(if applicable\) | on\_demand |  |
| variant\_unit\_name \(if applicable\) |  |  |

The green columns are required, the orange are able to be updated, the white cannot be updated and aren't required.

![](../../.gitbook/assets/image%20%282%29.png)

What if I leave an updateable field blank? Will it become zero/erase the previous content? Or can I remove the columns that I don't want to update.

## Import New Inventory

Coming soon

## Update Existing Inventory Details

Coming soon

