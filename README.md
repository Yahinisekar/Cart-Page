# Shopping Cart Component

This React component, `Cart`, is designed to display a shopping cart interface where users can view items, adjust quantities, and remove items from their cart.

## Features

- Display a list of items in the cart, including details like item name, description, brand, stock, rating, and thumbnail image.
- Users can adjust the quantity of each item in the cart by incrementing or decrementing the quantity using "+" and "-" buttons.
- Users can remove items from the cart by clicking the "Remove" button associated with each item.
- Display the total quantity of items in the cart.
- Display the total price of all items in the cart.
- Provide a "Proceed to Pay" button for users to navigate to the payment page or perform other checkout-related actions.

## Usage

To use this component in your React application:

1. Copy the `Cart.js` file into your project.
2. Import the `Cart` component into your desired parent component.
3. Wrap the parent component or any ancestor component with a context provider to provide the state for the cart. 

For example:

```jsx
import React, { useState } from 'react';
import Cart from './Cart';
import { MyContextProvider } from './MyContextProvider'; // Assuming you have a context provider

function App() {
  return (
    <MyContextProvider>
      <div>
        <h1>My Shopping Cart</h1>
        <Cart />
      </div>
    </MyContextProvider>
  );
}

export default App;
```