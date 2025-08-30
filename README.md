# Real-Time Sentiment Analysis Dashboard

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![ApexCharts](https://img.shields.io/badge/ApexCharts-3366CC?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyBmaWxsPSIjZmZmZmZmIiByb2xlPSJpbWciIHZpZXdCb3g9IjAgMCAyNCAyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj48dGl0bGU+QXBleGNoYXJ0cy5qczwvdGl0bGU+PHBhdGggZD0iTTEwLjQgMTAuNkwxMiA1LjhsMS42IDEuNiAxLjYtMy4yTDEyIDB6bTAgMi44bDEuNiAxLjYtMy4yIDEuNi0xLjYtMy4yem0uMiA4LjZsMS40LTQuMi0yLjgtNC4yTDQgMTcuOHptMy0xMS4yTDEyIDguMmwtMi44IDIuOCAyLjggMi44IDEuNi0xLjZ6bS4yIDguNmwxLjYtMy4yIDEuNiAzLjItMS42IDEuNi0xLjYtNC4yem0xLjQtNS42bDIuOC0yLjgtMi44LTQuMi0yLjggNC4yem0tNyA1十四章TDEyIDE5bDIuOCAyLjhoLTUuNnoiLz48L3N2Zz4=)
![GSAP](https://img.shields.io/badge/GSAP-88CE02?style=for-the-badge&logo=greensock&logoColor=white)

This project is a sophisticated, single-page web application that simulates a real-time customer sentiment analysis dashboard. It's built entirely on the front-end and uses data simulation to showcase a dynamic and interactive user interface for monitoring feedback across various platforms.


[![Screenshot-17.png](https://i.postimg.cc/pdnD0Ntp/Screenshot-17.png)](https://postimg.cc/qt4hR5qT)
[![Screenshot-18.png](https://i.postimg.cc/h40VZbNb/Screenshot-18.png)](https://postimg.cc/w37t7Jq7)
---
## ✨ Features

The dashboard is split into two main sections, each packed with features:

### 📊 Live Dashboard
* **Real-Time Feeds**: Displays incoming messages from multiple sources (Twitter, Amazon, etc.), categorized and updated live.
* **Dynamic Stats**: Key performance indicators are updated every second:
    * **Msgs/Min**: Tracks the current message velocity.
    * **Pos/Neg Ratio**: Shows the ratio of positive to negative messages.
    * **Top Platform**: Highlights the most active source of messages.
* **Overall Sentiment Trend**: An ApexCharts area chart visualizes the trend of positive, negative, confusion, and frustration sentiments over time.
* **Interactive Sentiment Heatmap**: Provides a color-coded overview of sentiment intensity across all platforms. Clicking a platform filters the entire live dashboard.
* **Instant Alerts**: A dedicated panel for important notifications, such as spikes in negative sentiment.

### 🔍 Analytics Deep Dive
* **Historical Breakdown**: A clickable bar chart showing the total volume of messages for each sentiment type. Clicking a bar filters the keyword clouds.
* **Sortable Platform Performance Table**: A detailed table comparing platforms by total messages and average sentiment score. All columns are sortable.
* **Dynamic Keyword Clouds**: Two sections displaying the top positive and negative keywords. These clouds update based on the emotion selected in the historical chart.

### 🌐 User Experience & Interface
* **Multi-language Support**: Easily switch between **English**, **Hindi**, and **Marathi** with a dropdown menu. All UI elements are translated instantly.
* **Sleek Glassmorphism UI**: A modern design using blurred backgrounds and subtle borders for a "glass card" effect.
* **Smooth Animations**: Powered by GSAP and CSS transitions for fluid interactions, including element fade-ins, modal pop-ups, and hover effects.
* **Responsive Design**: The interface is fully responsive and optimized for both desktop and mobile devices using Tailwind CSS.
* **Interactive Modal**: A functional "Create Account" modal demonstrates form handling and user feedback within the UI.

---
## 🛠️ Tech Stack

This project is built with modern front-end technologies and requires **no backend or build process**.

* **HTML5**: For the core structure and content.
* **Tailwind CSS**: A utility-first CSS framework for rapid UI development and responsive design.
* **Vanilla JavaScript (ES6+)**: For all application logic, data simulation, and DOM manipulation.
* **ApexCharts.js**: A powerful charting library for creating interactive and beautiful data visualizations.
* **GSAP (GreenSock Animation Platform)**: A professional-grade animation library for high-performance UI animations.

---
## 🚀 Getting Started

Since this is a self-contained front-end project, running it is incredibly simple.

### Prerequisites
You only need a modern web browser (like Chrome, Firefox, or Edge).

### Installation
1.  Clone the repository to your local machine:
    ```sh
    git clone [https://github.com/Sd8738/sentiment-dashboard.git]
    ```
2.  Navigate into the project directory:
    ```sh
    cd sentiment-dashboard
    ```
3.  Simply open the `sentiment.html` file in your web browser. That's it!

---
## 🏗️ Code Architecture

The entire application is encapsulated within the `sentiment.html` file. The JavaScript is logically structured into distinct sections for clarity and maintainability:

* **Data Simulation & Config**: Contains the static data (sources, emotions, sample messages) and translation strings that power the simulation.
* **UI Components & Templates**: Functions that generate HTML strings for dynamic elements like message cards.
* **Charting & Visualization**: Handles the initialization and updating of all ApexCharts instances.
* **Application Logic**: The core engine of the dashboard. It includes functions for:
    * Generating random messages.
    * Updating the DOM with new data.
    * Calculating live statistics.
    * Managing the real-time simulation loop (`realTimeLoop`).
* **Initialization & Navigation**: Sets up all event listeners, handles page switching, and kicks off the main loop when the DOM is loaded.

---
## 🔮 Future Enhancements

This project serves as an excellent foundation. Potential future improvements include:
* **Backend Integration**: Connect the dashboard to a real backend service (e.g., Node.js with WebSockets) to process and display live data from APIs like Twitter or a database.
* **User Authentication**: Implement a functional login system for the "Create Account" modal.
* **Date Range Filtering**: Add a date picker to the Analytics page to view historical data for specific periods.
* **Advanced Visualizations**: Introduce more complex chart types, such as word clouds or sunburst charts, for deeper insights.

---
## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.
