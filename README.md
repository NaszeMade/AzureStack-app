# AzureReact App - React Application Deployment on Azure

**Project Overview:**
Built and deployed a modern React application to Microsoft Azure using Webpack, Babel, and Azure Web Apps. This project demonstrates my ability to configure modern frontend tooling and deploy scalable web apps in the cloud.

## Key Features
- Configured React environment from scratch
- Customized Webpack and Babel for optimized build process
- Connected with Azure Web App for live deployment
- Fully responsive, production-ready React app
- Cloud-hosted with live URL and CI/CD potential

## Tools & Services Used
- React.js
- PostgreSQL
- Docker
- Svelte
- PM2
- Caddy
- freedns.afraid.org

## Getting Started
### Prerequisites
- Azure subscription
- VS Code

## Installation & Local Setup
1. Clone the repository:  
   `git clone https://github.com/naszemade/AzureReact-app`
   `cd AzureReact-app`
   
2. Install Dependencies:  
   `npx create-react-app`

3. Install Webpack Packages:  
   `npm install webpack webpack-cli webpack-dev-server babel-loader @babel/core @babel/preset-env @babel/preset-react html-webpack-plugin --save-dev`
   `npm install style-loader css-loader --save-dev`

4. Install Build Packages:  
   `npm run build`

5. Install
   `npm install -g serve`
   `serve -s build`
   
6. Run the Application
   `npm start`
   
## ☁️ Azure Deployment Steps
1. Create Azure Web App from Azure Portal
2. Set up your GitHub repo as deployment source
3. Configure build commands and output folder
4. Push to main branch and Azure deploys automatically

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact
Connect with me on [LinkedIn](https://www.linkedin.com/in/nasze-royster/)
For inquiries or concerns, please contact me via [GitHub](github.com/naszemade)
