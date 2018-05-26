.. _jamla_payment_providers:

Payment Providers
=====================

--------------------------------
Example payment providers jamla
--------------------------------

Except from :ref:`jamla-latest`

Payment Providers:: 

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
                 - environment: 'sandbox' 
