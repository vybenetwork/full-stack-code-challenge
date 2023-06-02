# Vybe Full-Stack Code Challenge

 ## Challenge Description

Your challenge is to create a simple React application with a Node API backend, both implemented in TypeScript. The application will interact with the Solana blockchain to fetch data and display this on various charts.

**Backend - Node API**

Your backend will be a Node.js server, which will interact with the Solana blockchain through the public RPC endpoint `https://solana-mainnet.rpc.extrnode.com/`. You will make use of the `getTokenSupply` and `getRecentPerformanceSamples` and `getBalance` RPC methods. Use the `@solana/web3.js` npm package to connect to the RPC server and call the methods. 

You should fetch data for five of your most bullish SPL tokens. For each token, you will fetch the current supply and use the price API `https://price.jup.ag/v4/price?ids=tokenMintAddress,tokenMintAddress` (replace tokenMintAddress with a comma separated list of token mint addresses) to calculate the market cap.

You should also fetch the Solana transactions-per-second (TPS) metric, and create endpoints for this data. You can refer to [Solana's Explorer Repo](https://github.com/solana-labs/explorer) for some inspiration on how TPS can be calculated.

**Frontend - React Application**

Your frontend application will fetch and display the backend data using three types of charts. The library to use for charts is up to you, but we suggest Apexcharts.js or Chart.js.

1. A pie chart that represents the market cap of each of your five chosen SPL tokens.
2. A time series chart that displays the Solana transactions per second (TPS) metric over time, you can decide on the interval and the time period you show on the chart. 
3. A bar chart that shows the wallet SOL balances of 10 different wallet addresses. You can choose these addresses randomly or based on your interest. For finding wallet addresses, you can use our [Rich List page](https://alpha.vybenetwork.com/tokens/richlist).

**Testing**

The application should include a basic suite of tests, at least covering the crucial functionality. Feel free to use Jest and Testing Library for this purpose. 

This is required for the React app, and optional for the Node API. 100% code coverage isn't expected, but you should provide at least 5 test cases.

**Development and Build Environment**

Your application should have a fully working development environment. Instructions should be provided on how to run the application in a development setting.

The frontend build environment should be set up using Vite, and it should compile the TypeScript code into a browser-compatible JavaScript bundle.

**Submission Guidelines**

Please submit your code in a GitHub repository. It should include:

1. Source code for the backend and frontend.
2. Test files.
3. A README file containing instructions on how to set up and run your application, including installing dependencies, running tests, starting the development server, and building the project.
4. Any additional documentation you feel necessary to understand your design and development decisions.

We expect this assignment to take around 4 hours to complete, please inform us if you find that you are spending a lot more time than that.

Remember, we're not just looking at if the final product works, but also your approach, code quality, choice of libraries, and general adherence to best practices. Good luck!
