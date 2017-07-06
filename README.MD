# eStarter. The beginning of your beautiful, custom ecommerce on Laravel.

## Features
- Create and organize categories & subcategoires
- Create attributes and group them in sets of attributes
- Create currencies
- Create carriers
- Create taxes and use them on products
- Create order statuses
- Create products and upload product multiple images on single time using dropzone
- Ability to create product groups
- Ability to clone a product

## Installation
- Clone repository
```
$ git clone git@github.com:updivision/estarter-ecommerce-for-laravel.git
```
- Run in your terminal
```
$ composer install
$ php artisan key:generate
```
- Setup database connection in .env file
```
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=homestead
DB_USERNAME=homestead
DB_PASSWORD=secret
```

- Migrate tables with demo data
```
$ php artisan migrate --seed
```

- Access it on
```
http://localhost/laravel-ecommerce/admin/login
```

## Setup
In order to the shop and be able to add products, you must have a minimum configuration:
- Create at least one category;
- Create at least one attribute for at least one of these types: text, textarea, date, dropdown, multiple select, media;
- Create at least one attribute set;
- Create a tax (eg. VAT).

After creating these, you’re ready to add your first product.

## Known Issues
- Product image uploader not fully responsive
- Changing attributes set on a product where old set has a media attribute type with an uploaded image and upload a new image to media attribute type cause an error
- Cloning a product does not clone values field from products_attributes_values table

## Roadmap for v1.0
- Implement orders
- Implement users management
- Improve product image uploader
- Improve and fix styles
- Cool ideas from developers :)