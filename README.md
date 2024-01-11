# Art Blocks On-Chain Generator Demo
This repository contains a demonstration application for the Art Blocks On-Chain Generator. This generator is a unique tool that assembles various on-chain resources, including project scripts, dependency scripts, and token data into a cohesive template. All of these components are stored on-chain. The generator leverages Scripty.sol to efficiently orchestrate the integration of these resources, producing the executable code needed to render an Art Blocks NFT in a web browser. The demo application retrieves the data URI of the NFT from a single contract call and injects it as the source of an iframe to display the token.

## Usage
Before running the application, you'll need to create a .env.local file in the root directory of the project and fill it with the variables specified in .env.example.

To run the application, use the following commands:

```
npm install
npm run dev
```

To view an NFT, navigate to `http://localhost:5173/<contract-address>/<token-id>`, replacing <contract-address> and <token-id> with the address of the NFT contract and the ID of the token you want to view. The application will fetch the data URI for the NFT and display it within an iframe.
