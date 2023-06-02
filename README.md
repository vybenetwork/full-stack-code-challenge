# Vybe Full-Stack Code Challenge

 ## Challenge Description

Your challenge is to create a simple React application with a Node API backend, both implemented in TypeScript. The application will interact with the Solana blockchain to fetch data and display this on various charts.

**Backend - Node API**

Your backend will be a Node.js server, which will interact with the Solana blockchain through the public RPC endpoint `https://solana-mainnet.rpc.extrnode.com/`. You will make use of the `getTokenSupply` and `getRecentPerformanceSamples` RPC methods. 

You should fetch data for five of your most bullish SPL tokens. For each token, you will fetch the current supply and use the price API `https://price.jup.ag/v4/price?ids=pid,pid` (replace pid with a comma separated list of addresses) to calculate the market cap.

You should also fetch the Solana transactions per second metric, and create endpoints for this data. 

**Frontend - React Application**

Your frontend application will fetch and display the backend data using three types of charts. The library to use for charts is up to you, but we suggest Apexcharts.js or Chart.js.

1. A pie chart that represents the market cap of each of your five chosen SPL tokens.
2. A time series chart that displays the Solana transactions per second metric over time.
3. A bar chart that shows the wallet balances of 10 different wallet addresses. You can choose these addresses randomly or based on your interest. For finding wallet addresses, you can use `https://solscan.io/`.

**Testing**

The application should include a basic suite of tests, at least covering the crucial functionality. Feel free to use Jest and Testing Library for this purpose.

**Development and Build Environment**

Your application should have a fully working development environment. Instructions should be provided on how to run the application in a development setting.

The frontend build environment should be set up using Vite, and it should compile the TypeScript code into a browser-compatible JavaScript bundle.

**Submission Guidelines**

Please submit your code in a GitHub repository. It should include:

1. Source code for the backend and frontend.
2. Test files.
3. A README file containing instructions on how to set up and run your application, including installing dependencies, running tests, starting the development server, and building the project.
4. Any additional documentation you feel necessary to understand your design and development decisions.

Remember, we're not just looking at if the final product works, but also your approach, code quality, choice of libraries, and general adherence to best practices. Good luck!
