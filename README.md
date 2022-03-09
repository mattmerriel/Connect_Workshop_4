# Content
# Amazon Connect with Voice ID and Wisdom

Welcome to the latest in my series of workshops around building Amazon Connect solutions. In this workshop we will look at add Voice ID and Wisdom to a contact centre solution for Phoney Bank, our 100% and not even remotely real bank.

## Who Are Phoney Bank
Phoney Bank is a Melbourne based, fintech start-up looking to break into the digital banking space. You've been hired as their lead developer and have been tasked with building out the infrastructure and services that will help them deliver modern banking services to their customers. You've been given complete freedom to build the stack however you see fit as long as it's run on AWS due to a partnership between the two companies.

## Current Business Problem
Today's focus is going to be on building out a phone based contact centre solution that will be used to service incoming requests for assistance from Phoney Bank customers. We need to:
- deploy a Contact centre solution on which we can accept incoming support calls
- implement a voice verification solution so that we can confirm a callers identity
- provide our support agents with access to a knowledge base of common customer queries to make supporting customers quicker and easier
To achieve this we can leverage three different AWS technologies.

Firstly we can use Amazon Connect to provide us with the centralised Contact Centre environment. This can provide us with a phone number for our customers to call and gives us a way for our support agents a way to interact with them.

Once we have our Connect Instance, we can then leverage a feature of Connect called Amazon Voice ID to help identify our callers by matching their voice print to one we'll have on file. While Voice Print matching is a powerful way to Identify a caller it won't be used as our sole mechanism for identification... just another piece in the authentication puzzle. In addition to identifying our customers, we can also use Voice ID to identify potential fraudulent callers to direct with agent to perform additional verification steps.

Once we've verified that a caller is who they say they are, we then need to help them get the information that they are after. Our customer support agents (those people who answer the incoming calls from customers) can have access to all our internal information (wiki's, Intranet, knowledge bases etc.) but they might not be quick to search meaning our customers will need to spend a lot of time waiting on the line while the answer is looked up. Luckily we can leverage Amazon Wisdom which is a content delivery system that can streamline the process of searching multiple locations for information and provide what the agent needs, right within the Connect Control Panel.

And that will just about do it... We'll have a contact centre our callers can ring into. We'll be able to verify their identity through the use of Voice Print matching using Voice ID. And we'll be able to quickly provide them with the information they are looking for by surfacing the information with Amazon Wisdom.

In the next section we'll get started with our new solution by standing up an Amazon Connect instance... The basis for the rest of the work we'll be doing today. 

Proceed to the next section [here](Part1.md)