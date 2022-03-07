# Challenge - Hooks

**hooks/useCart.tsx**

- Cart
  - [x] shold check if there is value in `@RocketShoes:cart`.
  - [x] if there is return items
  - [x] if not return empty array.
- Add Product
  - [x] shold add products to cart, but check if:
    - [x] use method `setItem` for perpetuate in localStorage.
    - [x] if the product there is in cart, only update amount unity.
    - [x] check that the inventory has the required value.
      - [x] if not have, use:
      ```javascript
      toast.error("Quantidade solicitada fora de estoque");
      ```
      - [x] catch mistakes during method if have error, use:
      ```javascript
      toast.error("Erro na adição do produto");
      ```
- Remove Product
  - [x] shold remove one product, but verify if:
    - [x] cart value update and perpetuate in localStorage.
    - [x] catch error and show message:
    ```javascript
    toast.error("Erro na remoção do produto");
    ```
- Update Product Amount.
  - [x] shold update the quantity of products in the cart, but:
    - [x] cart value update and perpetuate in localStorage.
    - [x] if the `quantity of product is <= 0`, exit the function.
    - [x] check that the inventory has the required value, if not have:
    ```javascript
    toast.error("Quantidade solicitada fora de estoque");
    ```
    - [x] catch error and show message:
    ```javascript
    toast.error("Erro na alteração de quantidade do produto");
    ```

**Header/index.tsx**

- [x] shold get the cart array from useCart (Context - Cart).
- [x] shold show the amount of products added to cart.


