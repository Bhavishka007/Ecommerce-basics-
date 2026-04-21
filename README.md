🛒 E-Commerce Product Gallery
A lightweight, dynamic e-commerce product display page built with Vanilla JavaScript, CSS Grid, and the FakeStore API. 
This project demonstrates how to fetch external data, handle asynchronous operations, and implement real-time search filtering.

🚀 Key Features
Asynchronous Data Fetching:= Uses the Fetch API to retrieve product data from a RESTful service.
Live Search:= Real-time filtering logic that updates the UI as the user types.
Responsive Grid:= A mobile-friendly layout using CSS Grid.
Dynamic DOM Injection:= Cleanly manages UI updates by clearing and rebuilding the product container.

🛠️ Technical Concepts Used
Term,                                                   Implementation in this Project
Fetch API,                         Used to make a network request to https://fakestoreapi.com/products.
Promises,                          Handled via .then() chains to process the JSON response from the server.
DOM Manipulation,                  Using document.createElement and append to build the UI entirely from JavaScript.
Higher-Order Functions,            Utilized .filter() for the search logic and .forEach() for rendering cards.
Event Handling,                    The oninput event listener triggers the search function instantly on every keystroke.
Data Persistence,                 "The bag variable acts as a local ""state"" to store the API response for faster filtering without re-fetching."
CSS Grid,                         "Defines a 4-column responsive layout with grid-template-columns: repeat(4, 1fr)."

📖 How It Works
Initialization:= On page load, a fetch request is sent to the API.
Storage:= The retrieved data is stored in a global array named bag to ensure we don't have to call the API every time a user searches.
Rendering:= The displayCart() function loops through the data, creates HTML elements (cards), and injects them into the #root div.
Filtering:= When a user types in the search bar, the search() function filters the bag array based on the category and re-renders only the matching items.

