# Pump.fun API

Trade any token on Pump.fun using the Solana Gateway Pump.fun API. With this API, you can buy and sell any token with higher rate limits and fast transactions using a simple POST request.

Optimized for quick transactions using bloXroute, it's ideal for sniping and purchasing tokens rapidly. There are no percentage fees, only a fixed system fee of 0.001 SOL per transaction.

## Why Choose Pump.fun API?

- Fast Transactions
- Best for Sniping
- Real-Time Price
- MEV Protection
- Low System Fee (0.001 SOL)
- No Hidden Fees or Charges
- Easy-to-Use API
- Detailed Documentation

## How to Buy and Sell Using the API

To buy, sell, or get real-time price information of a token, use the following API endpoints:

- **Buy:** `https://api.solanagateway.com/api/v1/pumpfun/buy`
- **Sell:** `https://api.solanagateway.com/api/v1/pumpfun/sell`
- **Price:** `https://api.solanagateway.com/api/v1/pumpfun/price`

### Required Parameters for Buying

- **private_key:** The main wallet to pay for the transaction and fee.
- **mint:** The token mint address of the token you want to purchase.
- **amount:** The amount in SOL (e.g., 0.001 or 1).
- **microlamports:** Default is set to 433000.
- **units:** Default is set to 300000.
- **slippage:** For example, 10 for 10% or 1 for 1%.
- **TIP:** A minimum of 0.001 is required for processing transactions faster via bloXroute validators. An additional system fee of 0.001 SOL is charged by the Solana Gateway.

### Required Parameters for Selling

- **private_key:** The main wallet to pay for the transaction and fee.
- **mint:** The token mint address of the token you want to sell.
- **amount:** The amount in tokens (e.g., 1 or 100000).
- **microlamports:** Default is set to 433000.
- **units:** Default is set to 300000.
- **slippage:** For example, 10 for 10% or 1 for 1%.
- **TIP:** A minimum of 0.001 is required for processing transactions faster via bloXroute validators. An additional system fee of 0.001 SOL is charged by the Solana Gateway.

### Required Parameters for Token Price Info

- **mint:** Token mint address using GET request

For more code examples or details, please visit: [Solana Gateway Documentation](https://docs.solanagateway.com/pump.fun-swap)

**Note:** This is not an official API by Pump.fun. This API is created by the Solana Gateway team, enabling you to create tools for yourself or the public. It is a reliable, fast, and secure API.
