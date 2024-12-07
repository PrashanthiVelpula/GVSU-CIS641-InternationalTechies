# GVSU-CIS641-International Techies

# HomeGoods Inventory Management

## Project description:

Our project, **HomeGoods Inventory Management**, is a comprehensive web application designed to streamline inventory management for store managers. The application features a secure login system that ensures only authorized users can access and manage the inventory.

Store managers can efficiently handle categories such as furniture, electronics, home decor, and more. The platform allows them to add, edit, and delete inventory items with ease. Each inventory item includes detailed information such as price, description, stock, and ratings to aid in effective management.

The backend leverages **Firebase**, offering reliable authentication, real-time data updates, and secure data storage. The frontend is built using **ReactJS**, styled with **HTML** and **CSS**, and enhanced with dynamic theming capabilities, including a **dark mode** option. These features focus on providing a user-friendly, responsive interface that simplifies inventory control, reduces manual effort, and boosts operational efficiency.

### Key Functionalities:

- **Dark Mode Support**: Provides a user-friendly interface that can adapt to light or dark themes based on user preferences.
- **Real-Time Inventory Updates**: Changes to inventory items (additions, edits, or deletions) are instantly reflected across all sessions.

This project represents a robust solution for inventory management, designed to scale with the needs of modern store managers.

## Team Members and Roles

* [SAI SURENDRA KOMMINENI](https://github.com/saisurendrakommineni/CIS641-HW2-KOMMINENI)
* [PRASHANTHI VELPULA](https://github.com/PrashanthiVelpula/CIS641-HW2-Velpula.git)
* [VENUKESWARI OOTLA](https://github.com/Venuootla/CIS-641-HW2-OOTLA)

## Prerequisites
- **React.js**: Familiarity with React components, hooks (like `useState`, `useEffect`), and props.
- **JavaScript (ES6+)**: Understanding of modern JavaScript features such as arrow functions, destructuring, and modules.
- **HTML/CSS**: Basic knowledge of HTML structure and CSS styling.
- **Firebase**: General understanding of Firebase services (e.g., Realtime Database, Authentication).

## Run Instructions
### **1. Development Environment**
1. **Install Visual Studio Code**  
   Download and install Visual Studio Code from [here](https://code.visualstudio.com/).
2. **Download and Install Node.js**  
   Download Node.js (which includes npm) from [here](https://nodejs.org/).

### **2. Clone the Project**
Clone the project repository to your local machine:

### **3. Install Dependencies**
Run the following commands to install the required packages:
```bash
npm install               # Installs project dependencies
npm install react-router-dom
npm install @fortawesome/react-fontawesome @fortawesome/free-solid-svg-icons
npm install firebase       # For backend integration
npm install -g firebase-tools  # Firebase CLI for deployment and management
```
### **4. Run the Application**
Start the development server using:
```bash
npm run dev                 # Access via http://localhost:<port>
```
### **5. Testing**
- Test the application locally.
- Verify features like adding/editing items and Firebase integration.

### **6. Deployment**
To deploy the application on GitHub Pages:
```bash
npm run deploy
```
This will deploy the application and create a `gh-pages` branch for GitHub Pages.


### Additional Information:
```bash
# Steps to Create React Application
npm create vite@latest > Enter Project_Name
cd Project_Name
npm install
npm run dev

# Deployment Using GitHub Pages
1. npm install gh-pages --save-dev
2. Add given lines before "build": "vite build" in package.json file.
	1. "predeploy": "npm run build",
	2. "deploy": "gh-pages -d dist",
3. Then in the vite.config.js file add this line before plugins: [react()]
	1. base: "/YOUR_REPOSITORY_NAME",
4. npm run deploy
5.New branch (gh-pages) will be created in which GitHub page is deployed.
```
## Links
- [Docs](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/tree/main/docs)
- [Meetings](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/tree/main/meetings)
- [Artifacts](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/tree/main/artifacts)
- [src](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/tree/main/src)
- [Tests](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/tree/main/tests)
- [Website](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/tree/main/website)
- [Project Proposal](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/blob/main/docs/proposal-template.md)
- [Software Requirements Specification](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/blob/main/docs/software_requirements_specification.md)
- [Final Software Requirements Specification](https://github.com/PrashanthiVelpula/GVSU-CIS641-InternationalTechies/blob/main/docs/software_requirements_specification_final.md)
## Deployment Link
[Final Project Deployment Link](https://prashanthivelpula.github.io/CIS_641_Final_Project/)
