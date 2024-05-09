
**_ Building an Shophere Ecommerce Website with Vanilla JavaScript _**




## Step 1: Selecting DOM Elements

- Use `document.querySelector()` to select the product container and template container elements from the HTML document.

## Step 2: Defining the Function

- Define a function named `showProductContainer` that takes an array of products as input.

## Step 3: Checking for Valid Input

- Check if the `products` array is truthy. If not, return `false`.

## Step 4: Iterating Over Products

- Iterate over each product in the `products` array using `forEach()`.

## Step 5: Destructuring Product Properties

- Destructure the properties of each product object (brand, category, description, etc.) for easier access.

## Step 6: Cloning the Template

- Use `document.importNode()` to clone the template container for each product.

## Step 7: Updating Product Information

- Update the cloned template with the product details:
  - Set the text content of elements to display product information.
  - Set the source attribute of the product image element.
  - Calculate and display the actual price based on the product price.

## Step 8: Adding Event Listener

- Add an event listener to a specific element (`.stockElement`) within each product template.
- Use event delegation to handle click events and pass relevant data (event, product id, stock) to the `homeQuantityToggle()` function.

## Step 9: Appending to Product Container

- Append the cloned template with updated product information to the product container element.

## Step 10: Ensuring Container Availability

- Check if the product container element exists before appending the cloned template.

## Conclusion

-  created a function that dynamically populates the product container with product information based on the provided array of products.


**_ # Steps to Define the homeQuantityToggle Function _**


# Steps to Define the homeQuantityToggle Function

## Step 1: Create a New JavaScript File

- Create `quantityToggle.js` to contain `homeQuantityToggle`.

## Step 2: Define the Function

- Define `homeQuantityToggle(event, id, stock)`.

## Step 3: Select Current Card Element

- Use `document.querySelector()` to select the card element based on `id`.

## Step 4: Retrieve Product Quantity

- Retrieve product quantity using `querySelector()`.

## Step 5: Parse Quantity Attribute

- Parse `data-quantity` attribute to an integer.

## Step 6: Handle Increment Event

- Increment quantity if event target is `"cartIncrement"` and quantity < stock.

## Step 7: Handle Decrement Event

- Decrement quantity if event target is `"cartDecrement"` and quantity > 1.

## Step 8: Update Product Quantity Display

- Update text content of product quantity element.

## Step 9: Update Quantity Attribute

- Set `data-quantity` attribute to new quantity.

## Step 10: Return Quantity

- Return updated quantity.

## Conclusion

You've created `homeQuantityToggle` in `quantityToggle.js`, enabling users to update product quantities interactively.

**_ Add To Cart Functionality _**


# Steps to Define the addToCart Function

## Step 1: Find Current Card Price and Quantity

- Select the current card element based on the provided `id`.
- Retrieve the product quantity from the current card element.
- Retrieve the product price from the current card element.

## Conclusion

You've defined the `addToCart` function, enabling users to add products to their cart with the provided quantity and price.

===================================================================
**_ Steps for Retrieving Cart Products from Local Storage _**
===================================================================

## Step 1: Incorporate `getCartProductFromLocalStorage` into `addToCart`

## Step 2: Define `getCartProductFromLocalStorage`

## Step 3: Retrieve Cart Products by using `localStorage.getItem()`

## Step 4: Check for Null or Undefined Cart Products

## Step 5: Parse Cart Products

## Step 6: Return Cart Products


**_ Steps to Update Product Price Before Adding to Local Storage _**


## Step 1: Extract Price Without Currency Symbol

- Use `replace()` to remove the currency symbol (`₹`) from the product price.

## Step 2: Calculate Total Price

- Multiply the extracted price by the product quantity to calculate the total price.

## Step 3: Prepare Product Data

- Create an object containing the product `id`, `quantity`, and updated `price`.

## Step 4: Add Product Data to Cart Array

- Push the product object to the existing cart array.

## Step 5: Convert Cart Array to JSON and Store in Local Storage

- Convert the updated cart array to JSON format using `JSON.stringify()`.
- Store the JSON string in local storage under a designated key.

