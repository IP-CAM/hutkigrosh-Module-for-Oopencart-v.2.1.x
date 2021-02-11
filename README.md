## Module for integration with CMS OpenCart 2.1.x

This module provides interaction between the online store based on CMS Opencart version 2.2.x and the payment service hutkigrosh.by
  * Integration module for version [OpenCart 1.5.x] (https://github.com/esasby/hutkigrosh-opencart1.5-module)
  * Integration module for version [OpenCart 2.2.x] (https://github.com/esasby/hutkigrosh-opencart2.2-module)
  * Integration module for version [OpenCart 2.3.x] (https://github.com/esasby/hutkigrosh-opencart2.3-module)
  * Integration module for version [OpenCart 3.0.x] (https://github.com/esasby/hutkigrosh-opencart3.0-module)

### Installation Instructions:
1. Create a backup of your store and database
2. Install the module [opencart21-hutkigrosh-payment-module.ocmod.zip] (https://github.com/esasby/hutkigrosh-opencart2.1-module/blob/master/opencart21-hutkigrosh-payment-module.ocmod. zip) using _Modules_ -> _Installing Extensions_
3. Opposite the HutkiGrosh module, click "Install" and then "Change".
4. Fill in the parameters to identify your store in the HutkiGrosh system
    * Unique identifier of the ERIP service - ID of the ERIP service
    * Login online store - login in the HutkiGrosh system.
    * Online store password - password in the HutkiGrosh system.
    * Path in the ERIP tree - the path for paying the invoice in the ERIP tree, which will be shown to the client after placing an order (for example, Payments> Store> Orders)
5. In the "Status" drop-down list, select "Enabled".
6. Save your changes.

### Attention!
To automatically update the status of the order (after the client pays the invoice issued to the ERIP), you must inform the technical support service of the "Hutki Grosh" service with the address of the processor:
``
http://mydomen.my/index.php?route=payment/hutkigrosh/notify
``

### Test data
To set up payment in test mode
 * use the data to connect to the test system, obtained during registration in HutkiGrosh
 * enable the "Sandbox" mode in the module settings
 * to emulate the payment by the client of the invoice, use the personal account of the [test system] (https://trial.hgrosh.by) (menu _ ERIP payment test_)

_Developed and tested with OpenCart v.2.1.0.2_ 
