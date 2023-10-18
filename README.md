# Match-Engine

Java 11 used (javac 11.0.18)

## Compilation:  

javac MatchingEngine.java

## Execution:    

java MatchingEngine

## Dependencies: 

Order.java, MarketOrder.java, LimitOrder.java

## Examples of inputs and outputs:

>>> limit buy 10 100
Order created: buy 100 @ 10.0 identifier_1
>>> limit buy 9 200         
Order created: buy 200 @ 9.0 identifier_2
>>> market sell 150
Trade, price: 10.0, qty: 100
Trade, price: 9.0, qty: 50
>>> limit sell 11 150
Order created: sell 150 @ 11.0 identifier_3
>>> edit order identifier_3 to 150 @ 9.9                        
Order cancelled
Order created: sell 150 @ 9.9 identifier_3
>>> limit buy 9.9 200
Trade, price: 9.9, qty: 150
Order created: buy 50 @ 9.9 identifier_4
>>> cancel order identifier_4
Order cancelled
>>> market buy 150
>>> market sell 150
Trade, price: 9.0, qty: 150
>>> 

