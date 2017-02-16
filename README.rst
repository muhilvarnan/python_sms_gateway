===================
Python SMS Gateway
===================

Python SMS Gateway is module used to send text sms. Currently the module supports following sms gateways

SMS Gateways
------------
 1. Nexmo

Installation
------------
 1.  pip install python_sms_gateway

Usage
-----
 1. Nexmo
       - Without Sender

            .. code-block:: python

               from python_sms_gateway.nexmo import NexmoConnector
               nexmo = NexmoConnector(api_key=XXXXXXX, api_secret=XXXXXXX)
               nexmo.send(to="+91xxxxxxxxxxx", text="hello")

       - With Sender

            .. code-block:: python

               from python_sms_gateway.nexmo import NexmoConnector
               nexmo = NexmoConnector(api_key=XXXXXXX, api_secret=XXXXXXX, sender="+91xxxxxxxxxx")
               nexmo.send(to="+91xxxxxxxxxxx", text="hello")