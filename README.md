# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png)  SOFTWARE ENGINEERING IMMERSIVE

## Getting started

1. Fork
1. Clone

Below is an array of objects:

```js
const products = [
  { model: "515", brand: "New Balance", color: "Green" },
  { model: "515", brand: "New Balance", color: "Yellow" },
  { model: "515", brand: "New Balance", color: "Blue" },
  { model: "515", brand: "New Balance", color: "Red" },
  { model: "574", brand: "New Balance", color: "Blue" },
  { model: "574", brand: "New Balance", color: "Red" },
  { model: "574", brand: "New Balance", color: "Pink" },
  { model: "574", brand: "New Balance", color: "Navy" },
  { model: "574", brand: "New Balance", color: "White" },
]
```

Let's start by connecting to the mongo interactive shell:

```sh
mongo
```

Next, let's create a new database:

```sh
use productsDatabase
```

Cool, now let's populate our products database with products. Let's start by creating a products collection, then using insertMany to insert multiple documents:

```sh
db.products.insertMany([
  { model: "515", brand: "New Balance", color: "Green" },
  { model: "515", brand: "New Balance", color: "Yellow" },
  { model: "515", brand: "New Balance", color: "Blue" },
  { model: "515", brand: "New Balance", color: "Red" },
  { model: "574", brand: "New Balance", color: "Blue" },
  { model: "574", brand: "New Balance", color: "Red" },
  { model: "574", brand: "New Balance", color: "Pink" },
  { model: "574", brand: "New Balance", color: "Navy" },
  { model: "574", brand: "New Balance", color: "White" },
])
```

Let's confirm that this insert many operation worked:

```sh
db.products.find({})
```

We should see all our products in our database.


Use the MongoDB lesson to solve for the following:

1. Find all New Balance 574 shoes.

```sh
<--- solution goes here !--->
```

2. Find all New Balance shoes that are either red or blue.

```sh
<--- solution goes here !--->
```

3. Insert 4 more New Balance shoes:

```sh
<--- solution goes here !--->
```

4. Update all navy New Balance shoes to Blue:

```sh
<--- solution goes here !--->
```

5. Delete all 515 New Balance shoes.

```sh
<--- solution goes here !--->
```

# Bonus

Create a better representation of a "product".

Maybe a product should have size, and size should be an array of sizes or perhaps a product should have a quantity.

For example:

```sh
{ model: "574", brand: "New Balance", color: "Red", sizes: [7,8,9,10,11], qty: 36 },
```

Once you have a better representation of a product, apply the changes to every product in the database.

Write your queries below:

```sh
<--- solution goes here !--->
```


