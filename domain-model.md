#Domain Models In Here
#User story1
```
As a user,
So I can find a specific cohort,
I want to search a list of all cohorts by a cohort name.
```


| Classes            |                            Methods								    | Scenario                  | Outputs     |
|--------------------|----------------------------------------------------------------------|---------------------------|------------ |
| `CohortRepository` |             `getCohortByName(String name)`                           |If cohort with name exists |Cohort object|                   
|                    |                                                                      |If cohort does not exist   | Null        |

#User story2
```
As a supermarket shopper,
So that I can pay for products at checkout,
I'd like to be able to know the total cost of items in my basket.
```

| Classes            |                            Methods								    | Scenario                  | Outputs     |
|--------------------|----------------------------------------------------------------------|---------------------------|------------ |
| `Basket`           |              `Total(Dictionary<string name, int price>)`             |Basket have items          |Total coast  |                   
|                    |                                                                      |Basket is empty            | false       |


#User story3
```
As an organised individual,
So that I can evaluate my shopping habits,
I'd like to see an itemised receipt that includes the name and price of the products
I bought as well as the quantity, and a total cost of my basket.
```


| Classes                    |                            Methods								    | Scenario                  | Outputs                                                     |
|----------------------------|----------------------------------------------------------------------|---------------------------|-------------------------------------------------------------|
| `Basket `                  |               `Product(name: String, price: Float, int quantity)`    | Create a product          |  Product object                                             |
|                            |                                                                      |                           |                                                             |
| `Item                   `  |              `AddReceiptItems(product)`                              |Basket have items          |  Receipt containing name, price, quantity and total cost    |                    
|                            |                                                                      |Basket is empty            |  string message                                             |
|                            |                                                                      |                           |                                                             |

