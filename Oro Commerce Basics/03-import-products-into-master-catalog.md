Import Products into the Master Catalog

You can add products to your OroCommerce master catalog in a couple of clicks. As you probably already have a .csv list of available products saved, you can adjust it to the OroCommerce's template and upload it to your master catalog.

To download the template and bulk upload your products:

Navigate to Products > Products in the main menu. The product list opens.
Click Import File on the top right.
In the Import dialog, click Choose File, select the required .csv file, and click Import File.
Click Export Template to download a sample .csv file with the necessary headers.
Create your bulk information in the .csv format based on the downloaded file. Once your file is ready, click Choose File, select the prepared .csv file, and click Import File.

https://hive.oroinc.com/wp-content/uploads/sites/21/2018/06/import_products-720x343-1.png

For our example, we have filled in the template with several simple products and provided the following information for them:

SKU (e.g., WRT1)
Attribute.Family.code  (e.g. default_family)
Status  (e.g., enabled)
Type  (e.g., simple)
Inventory_status.id  (e.g. in_stock)
Category.default.title (e.g., Presentation Equipment)
Names.Default.Value (e.g., Flipchart Easel 110)
PrimaryUnitPrecision.precision (e.g., 1)
 

https://hive.oroinc.com/wp-content/uploads/sites/21/2018/06/ImportProducts-1.png

 

Note: You can also validate your file before uploading it to check for errors. Click Validate to check your import results. If any Records have errors, fix them in the .csv file before starting the import.

Interactive status messages inform about the import progress, and once the import is complete, the changes are reflected in the list on refresh. Additionally, an email message with the import status is delivered to your mailbox.

Once the products are imported, they should become available on the product list in your application and inside their respective categories.


https://hive.oroinc.com/wp-content/uploads/sites/21/2018/06/imported-products-1536x549.png
https://hive.oroinc.com/wp-content/uploads/sites/21/2018/06/product-in-category-1536x581.png

Keep in mind that unless you create a web catalog to set the structure and design of your website, the structure of the master catalog will be used in the storefront. As you can see in the screenshot below, the four categories we have just added to the master catalog are now displayed in the storefront because we have no web catalog created to present the products yet.
