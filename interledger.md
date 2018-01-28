---
layout: default
title: "Interledger overview"
---
Interledger effectively removed the overhead of “routing” and removes it from both source and destination “nodes” and let’s the network determine how many and which “hops” are required for the funds to reach their destination. This solves the problem of the sender and receiver needing to be part of the same “network” (Mpesa, Bitcoin, USD etc.) and as long as participants agree to receive funds in a certain form, all of these “networks” can be joined together on the interledger 
into one big “internet of money”.

At a more technical level, the Interledger architecture is heavily inspired by the Internet architecture described in RFC 1122, RFC 1123 and RFC 1009 which was designed with similar principles in mind. 

Figure 1 - Interledger architecture

To connect to the IL, a sender or receiver need to interact through an application and a transport layer before the “ledgers” can speak to each other. Figure 1 illustrates a sender, receiver and “N” intermediary hops through various ledgers to facilitate a transaction. 

When a sender initiates the transaction a “destination” address must be defined. An example would be g.crypto.bitcoin.1BvBMSEYstWetqTFn5Au4m4GFg7xJaNVN2 or g.za.absa.bank.individual.4058893078. Details of how these addresses are constructed are available here.

# Example transaction flow

Leveraging the participants to construct a proof of concept transaction flow, lets say we had a customer using a payment app called “QuickPay”, which was a standalone retail payments application developed by wiGroup that allowed users to link their Luno BTC wallet, as well as ABSA bank account (coureousy of Waxd) to a simple payments app on their phone. If a customer wanted to transact in store they would simply open their application and a QR code representing a payment token issued by a token provider (let’s say wiCode) would appear on the screen. Now let’s say the customer wanted to purchase a R2.99 ice cream at Hungry Lion chicken outlet in Umtata Durban, which is a store integrated to the Eccentric payment switch. The user would generate their token, which would….
