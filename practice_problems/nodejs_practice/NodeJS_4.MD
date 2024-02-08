<h1 align = "center">Practical 11</h1>

- Create a file `index.js` 
- Now, using the `http` core module, create a web server that would handle requests to a **Used Goods Marketplace** SaaS product as detailed in the following questions

**Note**: The server must be running on port `8000` and display a message "Server initiated on port 8000..." when it the server is started


1. When a user navigates to the root URL of the web server, the server must display a message "Welcome to the BarterX"
2. When a user navigates to the `/products` URL, the server must display a message "Here are the products up for Sale in BarterX"
3. When a user naviages to the `/login` URL, the server must display a message "Login to the BarterX"
4. When a user navigates to the `/signup` URL, the server must display a message "Sign up to the BarterX"
5. When a user navigates to the `/profile` URL, the server must display a message "Trader Profile"
6. When a user navigates to the `/cart` URL, the server must display a message "Your Shopping Cart is here"
7. When a user navigates to the `/checkout` URL, the server must display a message "Lets' start shipping"
8. When a user navigates to the `/orders` URL, the server must display a message "Your Orders are here"
9. When a user navigates to the `/categories` URL, the server must display a message "Browse Categories"
10. When a user navigates to the `/chat` URL, the server must display a message "Your Chat with fellow Traders"
11. When a user navigates to the `/contact` URL, the server must display a message "Contact Us at"
12. When a user navigates to the `/about` URL, the server must display a message "The modern approach to trading our commodities"
13. For any other page, the server must display a message "Page not found"

Bonus: Maintain a `log.txt` file that keeps track of every request that the server receives along with details about the time and date of the request, request url
