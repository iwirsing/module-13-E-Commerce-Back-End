# Module 13 Object-Relational Mapping (ORM): E-Commerce Back End
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

##  Description:

This is a back end for an e-commerce using starter code. Express.js, Sequelize, MySQL, and DotEnv were technologies used.

##  Table of Contents 
1. [Installation](#installation)
2. [Usage](#usage) 
3. [Contributing](#contributing) 
4. [Screenshots](#screenshots)
5. [Walkthrough Video](#walkthrough-video)
6. [Test](#test) 
7. [Questions](#questions)
8. [License](#license)
9. [Sources](#sources)

## Installation 

1. Download the folder to the local computer. 
2. Open the folder in the terminal. 
3. Create a .env file to access one's local mysql database. The format is:
```
DB_NAME='ecommerce_db'
DB_PASSWORD='<your password here>'
DB_USER='root'
```
3. Run `npm i` to install the dependencies. 
4. Seed the database using `npm run seed` .
4. Finally run `node server.js` or `npm run start` to to run the program in the terminal.

## Usage 

Run `node server.js` in the terminal and  generate tests requests using Insomnia.

## Contributing 

Modify as needed according this project's license.

## Walkthrough Video

## Test 

Open Insomnia and create CRUD requests.

To test Categories:
1. GET http://localhost:3001/api/categories/ - to view all categories
2. GET http://localhost:3001/api/categories/3 - to view category by ID and in this test view category ID 3.
3. POST http://localhost:3001/api/categories/ with JSON body of 
`{"category_name": "Kitchen"}` - to create new category.
4. PUT http://localhost:3001/api/categories/6 with JSON body of `{"category_name": "Outdoor Stuff"}`- to update category with new name.
5. DELETE http://localhost:3001/api/categories/6 - to delete category ID 6

To test Products:
1. GET http://localhost:3001/api/products/ - to view all products
2. GET http://localhost:3001/api/products/2 - to view product by ID and in this test view product ID 2.
3. POST http://localhost:3001/api/products/ with JSON body of 
`{"product_name": "Volleyball",
"price": 75.00,
"stock": 3,
"tagIds": [4,5,6]}`- to create new product
4. PUT http://localhost:3001/api/products/6 with JSON body of 
`{"product_name": " Small Volleyball",
"price": 75.00,
"stock": 3,
"tagIds": [4,5,6]}`- to update existing product.
5. DELETE http://localhost:3001/api/products/6 - to delete product with ID 6

To test Tags:
1. GET http://localhost:3001/api/tags/ - to view all tags
2. GET http://localhost:3001/api/tags/2 - to view tags by ID and in this test view tag with ID 2.
3. POST http://localhost:3001/api/tags/ with JSON body of 
`{"tag_name": "leather"}`- to create new tag.
4. PUT http://localhost:3001/api/tags/9 with JSON body of 
`{"tag_name": "wood"}`- to update existing tag.
5. DELETE http://localhost:3001/api/tags/9 - to delete product with ID 6


## Questions? 

Please contact me through any of the following:

1. My [Github](https://github.com/iwirsing).
2. Email: <a href="mailto:ivymolina@gmail.com">ivymolina@gmail.com</a>

## License
    
The project in covered under the [MIT](https://opensource.org/licenses/MIT) license

## Sources
1. Tutor: Geronimo Perez
2. https://stackoverflow.com/
3. https://sequelize.org

