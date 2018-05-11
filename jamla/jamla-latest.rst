.. _jamla-latest:

Jamla latest
================

* Prices must always expressed in pence (e.g. £1 is 100).
* Strings may be wrapped in double or single quotes

Latest jamla.yaml::

	version: 1
	payment_providers:
		paypal:
			 - sepa_direct_supported: No
			 - subscription_supported: Yes
			 - instant_payment_supported: Yes
			 - variable_payments_supported: No
		stripe: 
			 - sepa_direct_supported: No
			 - subscription_supported: Yes
			 - instant_payment_supported: Yes
			 - variable_payments_supported: No
			 - publishable_key: ''
			 - secret_key: ''
		gocardless:
			 - sepa_direct_supported: No
			 - subscription_supported: Yes
			 - instant_payment_supported: Yes
			 - variable_payments_supported: Yes
			 - access_token: ''
			 - environment: ''

	items:
		- sku: adsl
		  title: ADSL
		  sell_price: 500
		  subscription: Yes
		  monthly_price: 1500
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
		- sku: fibre
		  title: Fibre
		  sell_price: 130
		  subscription: Yes
		  subscription_terms:
			  - minimum_term_months: 12
		  requirements:
			- instant_payment: Yes
			- subscription: Yes
			- customer_address: Yes
			- customer_contact_details_required: Yes
		  monthly_price: 130
		  selling_points:
			  - Super fast up to 40Mbps
			  - Friendly UK Support
			  - Unlimited Usage
		  icons:
			  - 
				  - src: images/fibre148.png
					size: 48x48
					type: image/png
				  - src: images/fibre192.png
					size: 192x192
					type: image/png 
