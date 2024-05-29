## MongoDB Day 1 Task

1.Find all the information about each products.

#### Query:

db. product. find()

### output screenshots:

![output screenshot](./assets/quest1-1.png)

![output screenshot](./assets/ques1%20-2.png)

![output screenshot](./assets/ques1-3.png)

![output screenshot](./assets/ques1-4.png)

![output screenshot](./assets/ques1-5.png)

 ![output screenshot](./assets/ques1-6.png)

![output screenshot](./assets/ques1-7.png)

 ![output screenshot](./assets/ques1-8.png)

  ![output screenshot](./assets/ques1-9.png)


 
 

2.Find the product price which are between 400 to 800.

#### Query:

db. product. find({product_ price:{$gte:400,$lte:800}})


### Output Screenshots:

  ![output screenshot](./assets/ques2-1.png)

   ![output screenshot](./assets/ques2-2.png)

 


3.Find the product price which are not between 400 to 600.

#### Query:

db.product.find({product_price:{$not:{$gte:400.$lte:600}}})

### Output Screenshots:

 ![output screenshot](./assets/ques3-1.png)

  ![output screenshot](./assets/ques3-2.png)

   ![output screenshot](./assets/ques3-3.png)

![output screenshot](./assets/ques3-4.png)

 ![output screenshot](./assets/ques3-5.png)

 ![output screenshot](./assets/ques3-6.png)

  ![output screenshot](./assets/ques3-final.png)

4.List the four product which are greater than 500 in price.

#### Query:

db. product. find({product_ price:{$gt:500}}).limit(4)

### Output Screenshots:

 ![output screenshot](./assets/ques4-1.png)

 


5.Find the product name and product material of each products.

#### Query:

 db.product.find({},{product_name:1,product_material:1,_id:0})

### Output Screenshots:

 ![output screenshot](./assets/ques5-1.png)
 
  ![output screenshot](./assets/ques5-2.png)

 ![output screenshot](./assets/ques5-3.png)

  ![output screenshot](./assets/ques5-4.png)

   ![output screenshot](./assets/ques5-5.png)

 

6.Find the product with a row id of 10.

#### Query: 

db.product.find({id:”10”})

### Output Screenshots:

 ![output screenshot](./assets/ques6-1.png)

 

7.Find only the product name and product material.

#### Query: 

db.product.find({},{product_name:1,product_material:1,_id:0})

### Output Screenshots:

 ![output screenshot](./assets/ques7-1.png)

 ![output screenshot](./assets/ques7-2.png)

  ![output screenshot](./assets/ques7-3.png)

 ![output screenshot](./assets/ques7-4.png)

  ![output screenshot](./assets/ques7-5.png)
 

8.Find all products which contain the value of soft in product material.

#### Query:

db.product.find({product_material:/soft/i})

### Output Screenshots:

 ![output screenshot](./assets/ques8-1.png)

  ![output screenshot](./assets/ques8-2.png)

 
9.Find products which contain product color indigo and product price 492.00.

There is no data exactly present at same id with product _color : ”indigo” and product_price:492.00

 ### Output Screenshot:

  ![output screenshot](./assets/ques9.png)

10.Delete the products which product price value are 28.

#### Query:

db. Product. findMany ({product_price:28})

Ans: row  9 Will get deleted

### Output Screenshots:

 ![output screenshot](./assets/ques10-1.png)

  ![output screenshot](./assets/ques10-2.png)

   ![output screenshot](./assets/ques10-3.png)
 


 





