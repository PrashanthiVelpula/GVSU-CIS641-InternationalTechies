# GVSU-CIS641-International Techies

## Project description:

Our project, **HomeGoods Inventory Management**, is a proposed web application aimed at streamlining inventory management for store managers. The application will provide a secure login system for authorized users, allowing them to efficiently manage categories such as furniture, electronics, and home decor. Store managers will be able to add, edit, and delete inventory items, with detailed pages displaying information like price, description, and ratings. The backend will be built using either Firebase or MongoDB, ensuring efficient data storage and real-time updates. The frontend will be developed using HTML, CSS, and ReactJS, with a focus on simplicity, flexibility, and enhanced inventory control to reduce manual effort and improve operational efficiency.

## Team Members and Roles

* Member 1 
- [SAI SURENDRA KOMMINENI](https://github.com/saisurendrakommineni/CIS641-HW2-KOMMINENI)
* Member 2 
- [PRASHANTHI VELPULA](https://github.com/PrashanthiVelpula/CIS641-HW2-Velpula.git)
* Member 3 
- [VENUKESWARI OOTLA](https://github.com/Venuootla/CIS-641-HW2-OOTLA)

## Prerequisites

## Run Instructions
## **Development Environment**
1. **Install Visual Studio Code**  
   Download and install Visual Studio Code from [here](https://code.visualstudio.com/).
2. **Download and Install Node.js**  
   Download Node.js (which includes npm) from [here](https://nodejs.org/).

## **Installation Packages**
Run the following commands to install the required packages:
```bash
npm install
npm install react-router-dom
npm install @fortawesome/react-fontawesome @fortawesome/free-solid-svg-icons
npm install firebase
npm install -g firebase-tools

##Additional Information:
### Steps to Create React Application

npm create vite@latest > Enter Project_Name
cd Project_Name
npm install
npm run dev

### Deployment Using GitHub Pages
1. npm install gh-pages --save-dev
2. Add given lines before "build": "vite build" in package.json file.
	1. "predeploy": "npm run build",
	2. "deploy": "gh-pages -d dist",
3. Then in the vite.config.js file add this line before plugins: [react()]
	1. base: "/YOUR_REPOSITORY_NAME",
4. npm run deploy
5.New branch (gh-pages) will be created in which GitHub page is deployed.
