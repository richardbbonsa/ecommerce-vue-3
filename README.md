# vue-3-ecommerce

Tienda online.

## Entities

### Product

- id
- name
- description
- price
- image



### Category

- name
- description


## ShoppingCart

- products `[
    {
        productID: 1,
        quantity: 3,
    },
    {
        productID: 7,
        quantity: 5,
    }
    ]`

## Components

## ProductCard

## Pages

- / -> all products
- /category/5 -> products only of category 5
- /cart -> view the shopping cart

## Project Setup

```sh
npm install
```

### Compile and Hot-Reload for Development

```sh
npm run dev
```

### Type-Check, Compile and Minify for Production

```sh
npm run build
```

### Lint with [ESLint](https://eslint.org/)

```sh
npm run lint
```
