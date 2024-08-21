# 🍕 Fast React Pizza Co.

This is a simple React application where users can order one or more pizzas from a dynamically loaded menu. The app is designed to be user-friendly, requiring minimal user input to place an order.

## 🚀 Features

- **Dynamic Pizza Menu**: The pizza menu is loaded from an API, allowing for changes in the available options without modifying the frontend.
- **Cart Functionality**: Users can add multiple pizzas to their cart before placing an order.
- **Simple Order Process**: Users only need to provide their name, phone number, and address to place an order.
- **GPS Location**: If possible, the app will automatically provide the user's GPS location to facilitate easier delivery.
- **Priority Order**: Users can mark their order as "priority" for an additional 20% of the cart price, even after the order has been placed.
- **Order Submission**: Orders are sent via a POST request to the API, including the user's data and selected pizzas.
- **Unique Order ID**: Each order receives a unique ID, allowing users to look up their order later.
- **No Payment Processing**: Payments are made on delivery, so no payment processing is needed within the app.

## 🛠️ Installation

To run this project locally, follow these steps:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/pizza-ordering-app.git
   ```
2. **Navigate to the project directory**:
   ```bash
   cd pizza-ordering-app
   ```
3. **Install dependencies**:
   
   Make sure you have [Node.js](https://nodejs.org/) installed, then run:
   ```bash
   npm install
   ```
4. **Start the development server**:
   ```bash
   npm run dev
   ```

After performing these steps, you should be able to access the application via the URL provided in the terminal output (probably http://localhost:5173).

## 🧩 Project Structure

- `src/features`: Contains core features of the app, including the pizza menu and cart functionality.
- `src/ui`: Contains React components that manage the user interface, such as forms, buttons, and other UI elements.
- `src/services`: Contains API service functions for loading the pizza menu and submitting orders.
- `src/utils`: Contains utility functions, such as generating a unique order ID.

## 🎨 Styling

The project uses Tailwind CSS for styling. Tailwind provides utility-first CSS classes that make it easy to style components directly in your JSX files.

To use Tailwind CSS in your project, ensure that you have it installed and properly configured in your `tailwind.config.js` file. You can refer to the [Tailwind CSS documentation](https://tailwindcss.com/docs/installation) for setup instructions.

## 📖 Usage

1. **Load Menu**: The menu is dynamically fetched from the API when the app loads.
2. **Add to Cart**: Users can select pizzas and add them to their cart.
3. **Provide Details**: Users enter their name, phone number, and address before submitting the order.
4. **Submit Order**: Once the order is submitted, a unique order ID is generated, and the order is sent to the API.
5. **Priority Option**: Users can mark their order as "priority" for an additional charge, even after placing the order.

## 🗺️ GPS Location (Optional)

If available, the app will attempt to use the device's GPS to automatically fill in the user's location details.
