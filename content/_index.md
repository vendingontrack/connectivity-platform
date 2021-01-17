---
title: Vending Machine API
subtitle: Connectivity Platform
comments: false
---

# Connectivity Platform


Vending on Track's Connectivity Platform is the only API for vending machines. 



By implementing a few API endpoints, businesses can integrate vending machines into their existing software and mobile apps, leveraging Vending on Track’s proven connectivity technology and experiences. It removes complexities to assist software developers in areas like hardware manufacturing, firmware development, backend platforms etc. 


This Connectivity Platform supercharges software businesses to focus on their core business activities, and this opens a vast range of opportunities for tech companies and developers who are interested in getting vending machines to communicate with their software or brands.



It opens doors for software developers to the  amazing world of IoT for vending machines.


Some use cases include,
* Coffee machine operators can easily integrate this technology to make operation more transparent and efficient while offering a branded experience for clients;
* Gyms can provide hydration and energy products to customers and encourage gym use;
* Construction and safety businesses can do monitored and controlled dispensing of PPE vending products with integrated safety mobile app technology;
* Digital wallets and payment gateways can connect to Vending on Track’s Connectivity Platform to increase their usage and popularity;
* The Buy-Now-Pay-Later market has grown enormously, and the demand for these companies to take full advantage of our system to improve their adoption rates is vast.


# API

The basic integration can be summaries by following chart,

![Sample Flow](/image/sample-flow.png)

These 7 steps will finish a basic transaction,
1. 3rd party starts the transaction by locking Connectivity Platform vending machine `/api/lock`
2. customer makes selection on vending machine
3. Connectivity Platform notifies 3rd party the selection by calling `/txn/request`
4. 3rd party keeps the book/journal, and approves the transaction by calling `/api/paid`
5. Connectivity Platform controls vending machine to dispense product to customer
6. customer picks up the product
7. Connectivity Platform notifies 3rd party the result of dispense by calling `/txn/vend`

----

For detailed information, please refer to 
* [Inbound API](/api/inbound_api.yaml) - Vending Machine API provided to 3rd party
* [Outbound API](/api/outbound_api.yaml) - 3rd party needs to implement this API for Connectivity Platform

Generated documents can be found here
* [Inbound API - generated HTML document](/api/inbound_api.yaml)
* [Outbound API - generated HTML document](/api/outbound_api.yaml)

