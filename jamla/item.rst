.. _jamla-item:

Item
=============

A Jamla item 
   Is an individual product or service. A valid 
   :ref:`jamla file<jamla-latest>` defines an `array` of products or 
   services you wish to sell on your shop. 

A single jamla item::
   
	- sku: adsl
	  title: ADSL
	  sell_price: 500
	  monthly_price: 1500
	  subscription: Yes
	  subscription_terms:
			  - minimum_term_months: 3
	  requirements:
			- instant_payment: Yes
			- subscription: Yes
			- customer_address: Yes
			- customer_contact_details_required: Yes
	  selling_points:
			  - Super fast up to 21Mbps
			  - Friendly UK Support
			  - Unlimited Usage
	- icons:                                                                         
	  -                                                                              
		  size: 48x48                                                                
		  src: images/adsl48x48.png                                                   
		  type: image/png                                                            
	  -                                                                              
		  size: 192x192                                                              
		  src: images/adsl192x192.png                                                   
		  type: image/png 
A Jamla item must include:


**sku**
  The stock keeping unit (sku) of the product or 
  service. `string`, `mandatory`
**title**
  Title of your product or service. `string`, `mandatory`
**sell_price**
  The upfront price of this product/service *expressed in pence*. This can be 
  left blank if there's no up-front cost for this item. `integer`, `optional`
**monthly_price**
  Monthly price of the product/service *expressed in pence*. This can be left 
  black if there's no monthly price. `integer`, `optional`
**requirements**
  The requirements of the item. `array`, `mandatory`
	**subscription**
	  Whether this item should take a reoccuring payment or not. 
	  `boolean`, `required`
	**instant_payment**
	  Whether this item should take a reoccuring payment or not. 
	  `boolean`, `required`
	**customer_address**
	  Item requires the customers address to be collected. `array`, `required`
	**customer_contact_details_required**
	  Item requires customer contactdetails to be collected. `boolean`, `required`
**subscription_terms**
  `array`
     **minimum_term_months**
        Minimum number of months this item can be purchased for. Useful for 
        services. `integer`, `optional`
**selling_points**
  Unique selling points of the item. `array`, `required`
**icons**
  Images of the item, with `src`, `type` and `size` for different screens. 
  `array`, `optional`
     
