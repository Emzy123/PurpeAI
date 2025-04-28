 # PurpleAI
     A website that uses AI to generate and deploy decentralized applications (dApps) and smart contracts across Web3 networks, featuring a futuristic purple-themed user interface.

     ## Overview
     PurpleAI simplifies Web3 development by allowing users to input natural language prompts to generate dApp and smart contract code, with a vibrant, purple-themed UI.

     ## Setup
     - Clone: git clone https://github.com/Emzy123/PurpeAI.git 
     - Install dependencies (to be added).
    
    - Commit:
   
     git add .
     git commit -m "Initialize PurpleAI project structure"
     git push origin main
     
     5. **Set Up Frontend (React)**:
     
     - Navigate to `client/`:
   
     cd client
     
     - Initialize a React project:
   

     npx create-react-app .
     
     - Start the development server:
     
     npm start
    
     - Open `http://localhost:3000` in your browser to verify the default React app.
     - Stop the server (Ctrl+C).
     
     - Commit:
   

     git add .
     git commit -m "Set up React frontend"
     git push origin main
    
    
    6. **Set Up Backend (Node.js)**:
    - Navigate to `server/`:
   

     cd ../server
     
     - Initialize a Node.js project:
   

     npm init -y
     
     - Install Express:
     
     
     npm install express
     
     - Create `server/index.js`:
   
    javascript
     const express = require('express');
     const app = express();
     const port = 5000;

     app.get('/', (req, res) => {
       res.send('PurpleAI Backend');
     });

     app.listen(port, () => {
       console.log(Server running at http://localhost:${port});
     });
     
    - Start the server:
     
     
    
     node index.js
    
     - Open `http://localhost:5000` to verify “PurpleAI Backend” appears.
     - Stop the server (Ctrl+C).
     
    - Commit:
     
     
    
     git add .
     git commit -m "Set up Express backend"
     git push origin main
    

    7. **Set Up Python Environment (for Future AI)**:
    - Navigate to `ai-model/`:
     
     
     cd ../ai-model
    
    - Create a virtual environment:
     
     
     python -m venv venv
    
    - Activate the virtual environment:
     - Windows: `venv\Scripts\activate`
     - macOS/Linux: `source venv/bin/activate`
     - Install basic AI libraries:
     
     
     pip install transformers torch
    
    - Deactivate: `deactivate`.
    - Commit:
     
     
     git add .
     git commit -m "Set up Python AI environment"
     git push origin main
    

    8. **Set Up Hardhat for Smart Contracts**:
    - Navigate to `contracts/`:
     
     

     cd ../contracts
    
        - Initialize a Node.js project:
     
     

     npm init -y
   
    - Install Hardhat:
     
     

     npm install --save-dev hardhat
   
    - Initialize a Hardhat project:
     
     

     npx hardhat
    
     - Select “Create a JavaScript project” and accept defaults.
    - Verify Hardhat:
     
     
     npx hardhat compile
    
     - Expected: No errors (will warn about no contracts yet).
    - Commit:
     
     
     git add .
     git commit -m "Set up Hardhat for smart contracts"
     git push origin main
    

    9. **Test Blockchain Access**:
    - Sign up for an [Infura](https://infura.io) or [Alchemy](https://alchemy.com) account.
    - Create a project and note the API key and endpoint (e.g., Sepolia testnet).
    - Create `server/.env` (not tracked):
     
    plaintext
        INFURA_API_KEY=your-infura-api-key
        
    - Verify MetaMask is installed and connected to the Sepolia testnet.
    - Commit `.env` placeholder (empty):
      
      
     touch .env
     git add .env
     git commit -m "Add .env placeholder for blockchain access"
     git push origin main
     
     10. **Final Commit**:
    - Return to the root folder:
    
      cd ..
     
    - Ensure all changes are committed:
    
      git add .
      git commit -m "Complete PurpleAI development environment setup"
      git push origin main
      `
