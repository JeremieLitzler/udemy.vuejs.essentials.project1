# Vuejs Essentials projects

## Projet 1

-  A `v-if` used along with a `v-else` must not be seperated semantically :

OK Example:

```html
<div v-if="cart.length" class="cart-total">
  Total: {{ cartTotal | currency }}
</div>
<div v-else class="empty-cart">
  No items in the cart.
</div>

```


KO Example:

```html
<transition name="fade">
  <div v-if="cart.length" class="cart-total">
    Total: {{ cartTotal | currency }}
  </div>
</transition>
<div v-else class="empty-cart">
  No items in the cart.
</div>

```

