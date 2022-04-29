# Step 01: Create-React-App
- npx create-react-app [project name]

# Step 02: Go to your package.json and add
- "homepage" : " . ",

# Step 03: Scripts
In the "scripts" section of package.json, add
- "pre-deploy": "npm run build" 
- "deploy": "npm run build && npm run deploy:arkb"
- "deploy:arkb": "arkb deploy build -w secrets/wallet.json --timeout=50000 --debug",

## Arweave pre-deploy

We will be using Arweave-deploy to package and deploy our site, as well as arkb. Enter the following commands to install them both:
- npm install -g arweave-deploy
- npm install -g arkb@latest
- Add your saved keyfile to a new directory /secrets with a name of wallet.json
* Remember to add to .ignore file if you use a version control


## Deployment
- npm run pre-deploy
- npm run deploy

All items will be deployed in a single bundle
Total size: 540.30 kB
Fees: 0.001071055174 + 0.000107105517 (10% arkb fee )
Total fee: 0.001178160691


Deployed on Arweave [Here](https://arweave.net/j_MJxCI0reXNHCsSJrFlRtDSQDNXdC9O1o6ZAuvrzwk)

txID: j_MJxCI0reXNHCsSJrFlRtDSQDNXdC9O1o6ZAuvrzwk
