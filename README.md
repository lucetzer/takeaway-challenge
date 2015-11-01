[![Build Status](https://travis-ci.org/makersacademy/takeaway-challenge.svg?branch=master)](https://travis-ci.org/makersacademy/takeaway-challenge)
[![CoverageStatus](https://coveralls.io/repos/lucetzer/takeaway-challenge/badge.svg?branch=master&service=github)](https://coveralls.io/github/lucetzer/takeaway-challenge?branch=master)

Takeaway Challenge
==================

Task
-----

The program is for a takeaway restaurant that allows customers to order dishes from a menu, check prices and total cost.
Completed orders will receive a SMS confirming when their order will be delivered. The key users stories are outlined below.

```
As a customer
So that I can check if I want to order something
I would like to see a list of dishes with prices

As a customer
So that I can order the meal I want
I would like to be able to select some number of several available dishes

As a customer
So that I can verify that my order is correct
I would like to check that the total I have been given matches the sum of the various dishes in my order

As a customer
So that I am reassured that my order will be delivered on time
I would like to receive a text such as "Thank you! Your order was placed and will be delivered before 18:52" after I have ordered
```

How to run the program
----------------------

1. Fork and clone this repo
2. Run ```bundle```
3. To test, run ```rspec```
4. Use irb in the command line to run this program. Example below:

```
$ require './lib/customer.rb'
$ customer_name = Customer.new
To create a new customer

$ customer_name.menu.pricelist
To see the menu and price

$ customer_name.make_order("dish", quantity)
To make an order

```

Technologies used
-----------------
* Ruby
* Testing using rspec
* Twilio API for text messaging functionality


Yet to do
---------
* Implement the ability to place orders via text message.
