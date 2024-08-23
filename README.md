# NTN Proof of Concept NIDD API

Non-IP Data Delivery (**NIDD**) provides a mechanism for simple asynchronous
messaging to a remote IoT device. NIDD messages provide small unstructured
binary payload, represented in the API as a hexadecimal string.

A user application is assigned to a private Access Point Name (**APN**) 
associated with an application *appId*. Viasat provides an API key upon
configuring the APN, to be used for authentication.
The user then registers three callback URLs where they establish HTTP
listener(s) to receive notifications, along with their inbound API key used by
the Viasat callback.

Mobile-terminated messages are submitted using a simple POST operation, then
the application receives a delivery notification via the pre-defined callback.

Contact Viasat to ask us more about our *Direct to Device*
*Early Adopter Program* (**DEAP**).