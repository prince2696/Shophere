🛒 Shophere – E-Commerce Website (Vanilla JavaScript)

A lightweight E-commerce web application built using pure JavaScript (no frameworks).
This project demonstrates DOM manipulation, event handling, localStorage usage, and dynamic UI rendering — ideal for mastering core JavaScript concepts.

✨ Features

✅ Dynamic product rendering using templates
✅ Quantity increment & decrement with stock control
✅ Add-to-Cart functionality
✅ Cart persistence using localStorage
✅ Clean, modular JavaScript structure

🚀 Product Rendering Workflow
🔹 Step 1: Select DOM Elements

Use document.querySelector() to target:

Product container

HTML template container

🔹 Step 2: Define showProductContainer()

Create a function that accepts an array of products and dynamically renders them on the page.

🔹 Step 3: Validate Input

Ensure the product list exists before proceeding:
if (!products) return false;

🔹 Step 4: Loop Through Products

Iterate using forEach() to handle each product individually.

🔹 Step 5: Destructure Product Data

Extract properties like:

.id
.brand
.category
.price
.stock
.description
.image

This improves readability and performance.

🔹 Step 6: Clone Template
Use document.importNode() to duplicate the product template for each item.

🔹 Step 7: Update Product Details

.Populate the cloned template with:

.Product name & description

.Image source

.Calculated price

.Stock availability

🔹 Step 8: Quantity Toggle (Event Delegation)

Attach a single click event to .stockElement:

.Handles increment & decrement

.Passes event, productId, and stock to homeQuantityToggle()

🔹 Step 9: Append to Container

Insert the updated product card into the product container.

🔹 Step 10: Safety Check

Ensure the product container exists before appending.

🎯 Quantity Management (homeQuantityToggle)

📁 File: quantityToggle.js

How It Works

Identify the clicked product card using id

Read the current quantity from data-quantity

Increment quantity (if stock allows)

Decrement quantity (minimum = 1)

Update UI & attributes in real-time

Return updated quantity

✔ Prevents over-ordering
✔ Ensures smooth UX

🔹 What Happens on Add to Cart?

Locate the selected product card

Fetch:

Product quantity

Product price

Prepare the data for cart storage

💾 Cart Persistence (Local Storage)
🔹 Retrieve Cart Products

Create getCartProductFromLocalStorage() to:

Access stored cart data

Handle empty cart scenarios

Parse JSON safely


🌟 Key Learnings
.DOM manipulation without frameworks

.Event delegation for performance

.Modular JavaScript architecture

.Persistent state using localStorage

📌 Ideal For

✔ JavaScript beginners
✔ Frontend interviews
✔ Portfolio projects
✔ Understanding core web fundamentals

🧑‍💻 Author

Prince Ranjan<br>
Frontend / Full-Stack Developer<br>
Focused on building scalable & clean web applications

<img width="1899" height="883" alt="image" src="https://github.com/user-attachments/assets/5734c5ce-d767-40ad-afcf-36c163010469" />

<img width="1903" height="883" alt="image" src="https://github.com/user-attachments/assets/e8fa4c2f-f545-4128-af64-7c20e80be3ee" />

<img width="1901" height="873" alt="image" src="https://github.com/user-attachments/assets/ebc20cd4-7bc9-4c97-bbf7-4a8ae2ddd7a5" />

<img width="1896" height="874" alt="image" src="https://github.com/user-attachments/assets/6f793fcb-41aa-4f74-aee5-ea4ac28ce5a2" />

<img width="1902" height="878" alt="image" src="https://github.com/user-attachments/assets/10844ed2-6fae-43cf-a6ba-d61b90f6d1aa" />

<img width="1902" height="885" alt="image" src="https://github.com/user-attachments/assets/55b51d9f-8405-4675-b58a-3ff377cf435c" />

<img width="1519" height="857" alt="image" src="https://github.com/user-attachments/assets/4a9579bd-b726-4d8b-8e2c-331d16a8a070" />

<img width="1874" height="833" alt="image" src="https://github.com/user-attachments/assets/91e97226-7f40-4b29-b023-e92456442a37" />









