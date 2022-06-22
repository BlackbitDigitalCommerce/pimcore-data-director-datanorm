# Datanorm export add-on for Pimcore Data Director

This bundle adds a result callback function template to Data Director's attribute mapping to create Datanorm exports. It defines virtual fields which you can map to your Pimcore data object fields. The result callback function already contains all the logic to create a Datanorm export file.

As it uses Data Director's export capabilities, your Datanorm exports profit by:
* everything is configurable in Pimcore backend user interface - no creation of PHP files or anything similar necessary
* access any data which is connected to exported products, for example you can easily access assigned categories, price information, manufacturers, product features etc.
* full flexibility in setting up a transformations like combining multiple Pimcore data object fields into one Datanorm field
* automatically execute exports whenever a product object gets saved whose data gets exported to:
    * prepare export once the data changes, so that the data does not have to be generated in the moment when the export is requested -> very fast exports because the export document is already available in the moment of request -> you will have an always up-to-date Datanorm export
    * upload exports automatically to a target system to always have up-to-date data there
    * automatically send data the other APIs
* intelligent checks whether anything changed since the last export. If nothing changed, export document gets delivered from cache
* access exports via URL, for example to pull Datanorm export into an external system instead of pushing it
* * *

## How to get the plugin

Please write an email to [info@blackbit.de](mailto:info@blackbit.de).