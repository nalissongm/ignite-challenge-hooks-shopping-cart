# Challenge - Hooks

**hooks/useCart.tsx**

- Cart
  - [x] shold check if there is value in `@RocketShoes:cart`.
  - [x] if there is return items
  - [x] if not return empty array.
- Add Product
  - [] shold add products to cart, but check if:
    - [] use method `setItem` for perpetuate in localStorage.
    - [] if the product there is in cart, only update amount unity.
    - [] check that the inventory has the required value.
      - [] if not have, use:
      ```javascript
      toast.error("Quantidade solicitada fora de estoque");
      ```
      - [] catch mistakes during method if have error, use:
      ```javascript
      toast.error("Erro na adição do produto");
      ```
- Remove Product
  - [] shold remove one product, but verify if:
    - [] cart value update and perpetuate in localStorage.
    - [] catch error and show message:
    ```javascript
    toast.error("Erro na remoção do produto");
    ```
- Update Product Amount.
  - [] shold update the quantity of products in the cart, but:
    - [] cart value update and perpetuate in localStorage.
    - [] if the `quantity of product is <= 0`, exit the function.
    - [] check that the inventory has the required value, if not have:
    ```javascript
    toast.error("Quantidade solicitada fora de estoque");
    ```
    - [] catch error and show message:
    ```javascript
    toast.error("Erro na alteração de quantidade do produto");
    ```

**Header/index.tsx**

- [] shold get the cart array from useCart (Context - Cart).
- [] shold show the amount of products added to cart.
