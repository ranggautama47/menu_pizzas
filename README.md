🍕 Fast React Pizza Co.

![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Create_React_App](https://img.shields.io/badge/Create_React_App-09D3AC?style=for-the-badge&logo=create-react-app&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)

A simple **React.js practice project** that displays a pizza restaurant menu.  
This project was created to practice **React fundamentals**, including components, props, conditional rendering, and dynamic list rendering.

## 📸 Preview

![Pizza Menu Preview](screenshot/menu.png)

## 🚀 Features

- Display a list of pizzas dynamically
- Show pizza name, ingredients, price, and image
- Conditional rendering for **sold-out pizzas**
- Dynamic rendering using **JavaScript `.map()`**
- Simple and clean UI using CSS
- Store open / close status based on current time

## 🧠 Concepts Practiced

This project focuses on learning important React concepts:

- React Components
- Props
- Conditional Rendering
- Rendering Lists with `.map()`
- JSX Syntax
- Basic Component Structure
- Simple State Logic (open/close time)

## 🏗️ Project Structure

```
📦 PIZZA-MENU
 ┣ 📂 node_modules
 ┣ 📂 public
 ┃ ┣ 📂 pizzas
 ┃ ┃ ┣ 📜 focaccia.jpg
 ┃ ┃ ┣ 📜 funghi.jpg
 ┃ ┃ ┣ 📜 margherita.jpg
 ┃ ┃ ┣ 📜 prosciutto.jpg
 ┃ ┃ ┣ 📜 salamino.jpg
 ┃ ┃ ┗ 📜 spinaci.jpg
 ┃ ┣ 📜 favicon.ico
 ┃ ┗ 📜 index.html
 ┣ 📂 src
 ┃ ┣ 📜 index.js
 ┃ ┗ 📜 index.css
 ┣ 📂 screenshot
 ┃ ┗ 📜 menu.png
 ┣ 📜 package.json
 ┗ 📜 README.md
```

## 🍕 Example Pizza Data

```javascript
{
  name: "Pizza Margherita",
  ingredients: "Tomato and mozzarella",
  price: 10,
  photoName: "pizzas/margherita.jpg",
  soldOut: false
}

Each pizza is rendered dynamically using:

pizzaData.map((pizza) => (
  <Pizza pizzaObj={pizza} key={pizza.name} />
))
```
## ⏰ Opening Hours Logic
```
The restaurant automatically checks if it is open:

const hour = new Date().getHours();
const openHour = 12;
const closeHour = 22;
const isOpen = hour >= openHour && hour <= closeHour;

If open, users can place an order.
If closed, a message will appear.
```

## 🎯 What I Learned

| Concept | Implementation |
|---------|---------------|
| Props | Passing `pizzaObj` to Pizza component |
| Conditional Rendering | `sold-out` class, ternary operators |
| List Mapping | `pizzaData.map()` with unique keys |
| Component Structure | App → Header, Menu, Footer |
| Dynamic Styling | Conditional CSS classes |
| Real-time Data | Restaurant open/close based on current hour |

## 🛠️ Technologies Used

| Technology | Badge | Description |
|------------|-------|-------------|
| React.js | ![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB) | UI library for component-based architecture |
| Create React App | ![CRA](https://img.shields.io/badge/CRA-09D3AC?style=flat-square&logo=create-react-app&logoColor=white) | Bootstrapped with CRA for zero-config setup |
| JavaScript (ES6+) | ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black) | Modern JS features like arrow functions, map, ternary |
| HTML5 | ![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white) | Semantic markup structure |
| CSS3 | ![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white) | Styling with modern CSS features |
| Google Fonts | ![Google Fonts](https://img.shields.io/badge/Google%20Fonts-4285F4?style=flat-square&logo=google-fonts&logoColor=white) | Roboto Mono for beautiful typography |

## 📦 Installation
```
Clone the repository:

git clone https://github.com/ranggautama47/menu_pizzas.git

Go to the project folder:

cd menu_pizzas

Install dependencies:

npm install

Run the project:

npm start

The application will run at:

http://localhost:3000
```
## 🎯 Learning Purpose

This project was built as part of my React learning journey to understand how to structure components and render dynamic content in React.


## 👨‍💻 Author

**Rangga Utama**  

[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ranggautama47)

## ⭐ Show Your Support

If this project helped you understand React props & state better, please give it a ⭐ — it motivates me to create more learning resources!

## Happy Coding! 🚀