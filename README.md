# AzureStack App - Full-Stack Cloud Deployment

**Project Overview:**  
AzureStack App project demonstrates the process of deploying a Node.js backend with a PostgreSQL database, a Svelte frontend, and a Caddy web server on a Microsoft Azure Virtual Machine. The goal is to create a fully functional web application that routes traffic securely and ensures seamless integration between components.

## Key Features
- **Backend Setup**: Built a Node.js backend and containerized the PostgreSQL database using Docker.
- **Frontend Deployment**: Developed and deployed a Svelte frontend, ensuring a responsive user interface.
- **Traffic Management**: Configured Caddy as a web server to efficiently route traffic between the frontend and backend services.
- **Domain Management**: Set up a free domain using freedns.afraid.org, ensuring accessibility via a custom URL.
- **Process Management**: Used PM2 to manage and monitor the backend process, ensuring continuous uptime.

## Tools & Services Used
- Azure Virtual Machine
- Node.js
- PostgreSQL
- Docker
- Svelte
- PM2
- Caddy
- freedns.afraid.org

## Steps to Implement
1. **Azure Virtual Machine Setup**  
   Provision an Azure Virtual Network (VNet) with multiple subnets.
  
2. **On-Premises Network Simulation**  
   Create a second VNet to simulate your on-premises environment.
  
3. **Secure Connectivity**  
   Establish a site-to-site VPN connection between the VNets.
  
4. **Resource Deployment**  
   Deploy VMs in each subnet for testing.
  
5. **Network Access Control**  
   Define access rules with NSGs.
  
6. **Secure Administrative Access**  
   Use Azure Bastion for RDP and SSH.
  
7. **Private Access to Azure PaaS**  
   Access Azure PaaS services via Private Link.
  
8. **DNS and Load Balancing**  
   Configure Azure DNS and implement a Load Balancer.
  
9. **Performance Testing**  
   Conduct tests to validate performance and security.
  
10. **Monitoring and Auditing**  
    Enable monitoring and review logs for security insights.

## Getting Started
### Prerequisites
- Azure subscription
- Basic understanding of Azure networking concepts
- Admin access to configure VPN gateways and networks

### Installation
1. Clone the repository:  
   `git clone https://github.com/naszemade/AzureStack-app`
   `cd full-stack-azure-deployment`
   
2. Install Dependencies for the backend:  
   `cd backend`
   `npm install`
3. Set Up PostgreSQL Database with Docker
   `docker run --name postgres -e POSTGRES_PASSWORD=yourpassword -d postgres`

4. Install Frontend Dependencies
   `cd frontend`
   `npm install`

5. Build and Deploy the Application
- Build the Node.js backend:
  `npm run build`
- Build the Svelte frontend:
  `npm run build`
   
6. Configure Caddy for Traffic Management
    `caddy reverse-proxy --from yourdomain.com --to localhost:3000` 
   
7. Domain Setup
   `caddy reverse-proxy --from yourdomain.com --to localhost:3000`
8. Run the Application with PM2
   `pm2 start server.js`
   
## Steps to Set Up the Project
1. [Azure Virtual Machine Setup](./docs/1-azure-vm-setup.md)
2. 

## Requirements
- Azure Subscription: Required to deploy the app on an Azure Virtual Machine.
- Docker: For containerizing the PostgreSQL database.
- Node.js: Backend runtime environment.
- PostgreSQL: Relational database management system.
- Svelte: Frontend framework.
- Caddy: Web server for reverse proxy and traffic routing.
- PM2: Process manager for keeping backend services running.
- freedns.afraid.org: For domain management and linking to Azure VM.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact
For inquiries, please contact me on [GitHub](github.com/naszemade)
