## Your eCommerce business needs to keep track of products and their prices. The products each belong to a department. The business needs to keep track of revenue as product prices change over time. The business also needs to keep track of receipts of transactions and the number of units each product has in stock.


## product

{
  * type: product
  * productId: integer
    * UPC
  * ProductName: string
  * PriceInfo: {
    * Price: integer
    * date: dateTime

  }
  * department: integer
  * Number of items in stock: integer
  * number of items sold: integer


}

## department

{
  * type: department
  * departmentId: integer
  * departmentName: string
  * products: [ array of product.productId ]

}

## transactions

{
  * type: transactions
  * transactionId: integer
  * Date: dateTime
  * items sold: [ array of product.productId ]
  * total price: integer

}
