🍽️ Restaurant Website – Food Ordering Interface

A responsive and interactive restaurant website developed using React.js, JavaScript, HTML5, and CSS3. The project provides a user-friendly interface for exploring food items, browsing menu categories, and managing shopping cart items.

📌 Project Overview

The Restaurant Website is a frontend web application designed to provide an engaging online experience for restaurant customers.

The application is developed using React.js with a component-based architecture. It includes dedicated components for food menu exploration, food item displays, navigation, login interface, and shopping cart management.

The project also uses the React Context API to share cart information and manage item quantities across different components.

Vite is used as the frontend development and build tool.

✨ Features

- Responsive restaurant website interface.
- Food menu and category exploration.
- Food item display using reusable React components.
- Restaurant header and navigation.
- Login popup interface.
- Shopping cart state management.
- Add food items to the cart.
- Increase item quantity when adding an existing item.
- Decrease item quantity using the remove function.
- Shared application state using React Context API.
- Food images and other visual assets.
- Separate pages for Home and Blogs.
- Organized and reusable component structure.

🛠️ Technologies Used

Technology| Purpose
React.js| Frontend development
JavaScript| Application functionality
HTML5| Webpage structure
CSS3| Styling and responsive design
React Context API| Shared state management
React Hooks| State and side-effect management
Vite| Development server and build tool
ESLint| Code quality and linting
Git| Version control
GitHub| Source code hosting

📂 Project Structure

Impact_Project/
│
└── frontend/
    │
    ├── public/
    │   ├── header_img
    │   └── vite.svg
    │
    ├── src/
    │   │
    │   ├── assets/
    │   │   ├── food images
    │   │   ├── menu images
    │   │   ├── header image
    │   │   ├── logo
    │   │   ├── cart and basket icons
    │   │   ├── profile and login icons
    │   │   └── other UI assets
    │   │
    │   ├── components/
    │   │   ├── ExploreMenu/
    │   │   ├── FoodDisplay/
    │   │   ├── FoodItem/
    │   │   ├── Footer/
    │   │   ├── Header/
    │   │   ├── Library/
    │   │   ├── LoginPopup/
    │   │   └── navbar/
    │   │
    │   ├── context/
    │   │   └── StoreContext.jsx
    │   │
    │   ├── pages/
    │   │   ├── Blogs/
    │   │   └── home/
    │   │
    │   ├── App.jsx
    │   ├── index.css
    │   └── main.jsx
    │
    ├── index.html
    ├── package.json
    ├── package-lock.json
    ├── .eslintrc
    └── vite.config.js

📁 Main Components and Their Responsibilities

1. ExploreMenu

Provides an interface for exploring different food menu categories.

2. FoodDisplay

Organizes and displays food items in the restaurant interface.

3. FoodItem

A reusable React component for displaying individual food items.

4. Header

Displays the main restaurant header section.

5. Navbar

Provides navigation between different website sections.

6. LoginPopup

Contains the login popup interface.

7. Footer

Displays the website footer section.

8. StoreContext – Shopping Cart Management

The project uses the React Context API to manage and share shopping cart information across different components.

Implemented functionality:

- Maintains cart item quantities using React "useState()".
- Adds food items to the cart using the "addToCart()" function.
- Increases the quantity when an existing item is added again.
- Decreases item quantity using the "removeFromCart()" function.
- Shares cart information and functions with child components through "StoreContext.Provider".
- Uses "useEffect()" to monitor changes in cart state.

React concepts used:

- "createContext()"
- "useState()"
- "useEffect()"
- Context Provider
- State management
- Component communication

9. Pages

Contains separate website page sections, including:

- Home
- Blogs

🛒 Shopping Cart State Management

The shopping cart functionality is implemented using React Context API.

The cart stores item quantities using an object-based state structure.

Example:

const [cartItems, setCartItems] = useState({});

Adding an item:

const addToCart = (itemId) => {
    if (!cartItems[itemId]) {
        setCartItems((prev) => ({
            ...prev,
            [itemId]: 1
        }));
    } else {
        setCartItems((prev) => ({
            ...prev,
            [itemId]: prev[itemId] + 1
        }));
    }
};

Removing an item:

const removeFromCart = (itemId) => {
    setCartItems((prev) => ({
        ...prev,
        [itemId]: prev[itemId] - 1
    }));
};

This approach allows multiple components to access and update cart information through the shared context.

⚙️ Installation and Setup

Follow these steps to run the project on your local machine.

Step 1: Clone the Repository

git clone https://github.com/Rajesh02092003/Impact_Project.git

Step 2: Navigate to the Frontend Directory

cd Impact_Project/frontend

Step 3: Install Dependencies

Make sure Node.js and npm are installed on your system.

npm install

Step 4: Start the Development Server

npm run dev

Step 5: Open the Application

After starting the development server, Vite will display a local URL in your terminal.

Open that URL in your web browser to access the website.

🎯 Project Objectives

- To develop a responsive restaurant website using React.js.
- To create reusable and maintainable UI components.
- To organize food menu categories and food item displays.
- To implement shopping cart state management.
- To understand React Context API and React Hooks.
- To improve frontend development and user interface design skills.

📚 Learning Outcomes

Through this project, I gained practical experience in:

- React.js fundamentals and component-based architecture.
- JavaScript and frontend development.
- Creating reusable React components.
- Managing shared state using React Context API.
- Using React Hooks such as "useState()" and "useEffect()".
- Implementing shopping cart quantity management.
- Organizing frontend assets and project folders.
- Building responsive user interfaces.
- Using Vite for frontend development.

🚀 Future Enhancements

- Improve the overall user experience and responsive design.
- Add food search and filtering functionality.
- Improve shopping cart quantity validation.
- Add automatic removal of items when their quantity reaches zero.
- Implement user authentication.
- Integrate backend services and database functionality.
- Add online ordering and payment integration.

👨‍💻 Author

Komali Rajesh

B.Tech – Computer Science and Engineering

- GitHub: "Rajesh02092003" (https://github.com/Rajesh02092003)
- LinkedIn: "Komali Rajesh" (https://www.linkedin.com/in/komali-rajesh-869817266/)

🔗 Project Repository

"Restaurant Website – Impact Project" (https://github.com/Rajesh02092003/Impact_Project)

---

⭐ If you find this project interesting, feel free to explore the repository!
