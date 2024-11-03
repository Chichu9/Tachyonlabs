# Configuration

The \`env\` file is where you configure the settings for the Tachyon Copybot. Below is a detailed explanation of each setting

#### General Settings <a href="#general-settings" id="general-settings"></a>

**LICENSE\_KEY**

* **Description**: Your unique license key to authorize the use of the Tachyon Copybot.
* **Example**: `LICENSE_KEY=your_license_key_here`

**PRIVATE\_KEY**

* **Description**: The private key of your Solana wallet. This key remains on your computer and is never sent or stored externally.
* **Example**: `PRIVATE_KEY=your_private_key_here`

**copy\_wallets.txt**

* **Description**: The list of wallets you want to copy trades from, each wallet (Base58-encoded string) on a new line. Unlike other copytrading bots that limit the number of wallets that you can copy, Tachyon Copybot allows you to copytrade an unlimited number of wallets!
* **Example**:

```
[ 
 { "wallet": "AAAAAAAXXXXXXXXXXXXXXXXXXX", 
 "buyAmount": 0.05, 
 "buySlippage": 300, 
 "sellSlippage": 70 
 } ,
 { "wallet": "BBBBBBBBBBXXXXXXXXXXXXXXXX", 
 "buyAmount": 0.05, 
 "buySlippage": 300, 
 "sellSlippage": 70 
 } ,
 { "wallet": "CCCCCCCCCCXXXXXXXXXXXXXXXXX", 
 "buyAmount": 0.05, 
 "buySlippage": 300, 
 "sellSlippage": 70 
 } 
]
```

**excluded\_wallets.txt**

* **Description:** The list of wallets you want to exclude from copying. Copybot will automatically detect token transfers and copy the recipient wallet for you. In some cases, the wallet you are copying may transfer tokens to a CEX, Raydium, or other address that you do not wish to copy. Please add these wallets to this list.
* **Example:**

```
[ 
 { "wallet": "AAAAAAAXXXXXXXXXXXXXXXXXXX", 
 } ,
 { "wallet": "BBBBBBBBBBXXXXXXXXXXXXXXXX", 
 } ,
 { "wallet": "CCCCCCCCCCXXXXXXXXXXXXXXXXX", 
 } 
]
```

**COMMITMENT\_LEVEL **_**(optional)**_

* **Description**: The level of commitment to use for Solana transactions. Common values are "processed", "confirmed", and "finalized".
* **Default**: `COMMITMENT_LEVEL=confirmed`

#### RPC Settings <a href="#rpc-settings" id="rpc-settings"></a>

**USE\_GRPC **_**(optional)**_

* **Description**: Determines whether to use gRPC (Geyser) for faster performance.
* **Default**: `USE_GRPC=false`
* **Example**: `USE_GRPC=true`

**GRPC\_ENDPOINT **_**(optional)**_

* **Description**: The endpoint for gRPC (Geyser) if you choose to use it.
* **Example**: `GRPC_ENDPOINT=your_grpc_endpoint_here`

**GRPC\_TOKEN **_**(optional)**_

* **Description**: The authentication token for your gRPC (Geyser) endpoint
* **Example**: `GRPC_TOKEN=your_grpc_token`

**RPC\_ENDPOINT**

* **Description**: The main RPC endpoint for connecting to the Solana blockchain.
* **Example**: `RPC_ENDPOINT=https://api.mainnet-beta.solana.com`

**RPC\_WEBSOCKET\_ENDPOINT**

* **Description**: The WebSocket endpoint for receiving real-time updates from the Solana blockchain.
* **Example**: `RPC_WEBSOCKET_ENDPOINT=wss://api.mainnet-beta.solana.com`

#### Bot Settings <a href="#bot-settings" id="bot-settings"></a>

**ONE\_TOKEN\_AT\_A\_TIME**

* **Description**: If set to `true`, the bot will trade one token at a time.

**USE\_JITO **_**(optional)**_

* **Description**: By default, copybot will send the transaction using Jito. If you do not want to use Jito, you can set this option to false. If both USE\_JITO and USE\_DEFAULT are both set to _false_, no transaction will be sent. If both are set to _true_, the transaction will be sent with both executors.
* **Default**: `USE_JITO=true`

**USE\_DEFAULT **_**(optional)**_

* **Description**: By default, copybot will send the transaction using Jito. If you would like to use default RPC transaction, you should set USE\_DEFAULT=true. If both USE\_JITO and USE\_DEFAULT are both set to _false_, no transaction will be sent. If both are set to _true_, the transaction will be sent with both executors.
* **Default**: `USE_DEFAULT=false`

**CUSTOM\_FEE**

* **Description**: Copybot retrieves the optimal Jito tip, but when there are connectivity issues that prevent the optimal Jito tip from being retrieved, the CUSTOM\_FEE will be used instead.
* **Example**: `CUSTOM_FEE=0.0001`

**JITO\_TIP\_PERCENTILE**

* **Description**: Copybot retrieves the optimal Jito tip and updates it every minute to ensure that your transactions land quickly and also prevent you from tipping more than you have to. You can set the percentile for the Jito tip here, with 25 being the lowest and 99 being the highest. The available options are: 25, 50, 75, 95, 99, ema
* **Example**: `JITO_TIP_PERCENTILE=75`

**DELAY\_BETWEEN\_RETRIES **_**(optional)**_

* **Description**: The delay (in milliseconds) between retry attempts for failed transactions. If you have set retries, the copybot will wait for this amount of time to receive confirmation of a successful transaction before retrying the transaction.
* **Default**: `DELAY_BETWEEN_RETRIES=1000`

#### Buy Settings <a href="#buy-settings" id="buy-settings"></a>

**QUOTE\_AMOUNT**

* **Description**: The amount of wSOL to use for each buy order.
* **Default**: `QUOTE_AMOUNT=0.02`

**MAX\_BUY\_RETRIES**

* **Description**: The maximum number of retries for buy orders. In the event that your transaction fails, the copybot will retry the transaction this many times.
* **Example**: `MAX_BUY_RETRIES=1`

**BUY\_SLIPPAGE **_**(optional)**_

* **Description**: The slippage percentage for buy orders. Higher slippage allows for more price variation.
* **Default**: `BUY_SLIPPAGE=80`

**BUY\_JITO\_FEE **_**(optional)**_

* **Description**: Here you can set the maximum Jito fee for buy orders. If the dynamically updated Jito fee exceeds this amount, this is the maximum amount that will be used as Jito tip for buy orders.
* **Default**: `BUY_JITO_FEE=0.0001`

#### Sell Settings <a href="#sell-settings" id="sell-settings"></a>

**AUTO\_SELL **_**(optional)**_

* **Description**: If set to `true`, the bot will automatically sell tokens when the copywallet sells.
* **Default**: `AUTO_SELL=true`

**MAX\_SELL\_RETRIES **_**(optional)**_

* **Description**: The maximum number of retries for sell orders.
* **Default**: `MAX_SELL_RETRIES=10`

**SELL\_SLIPPAGE **_**(optional)**_

* **Description**: The slippage percentage for sell orders. Higher slippage allows for more price variation.
* **Default**: `SELL_SLIPPAGE=70`

**SELL\_JITO\_FEE **_**(optional)**_

* **Description**: Here you can set the maximum Jito fee for sell orders. If the dynamically updated Jito fee exceeds this amount, this is the maximum amount that will be used as Jito tip for sell orders.
* **Default**: `SELL_JITO_FEE=0.001`

#### Market Settings <a href="#market-settings" id="market-settings"></a>

**RAYDIUM **_**(optional)**_

* **Description**: If set to `true`, the bot will copytrade on the Raydium platform.
* **Default**: `RAYDIUM=true`

**PUMPFUN **_**(optional)**_

* **Description**: If set to `true`, the bot will copytrade Pump.fun tokens on the bonding curve.
* **Default**: `PUMPFUN=false`

By understanding and configuring these settings, you can customize the Tachyon Copybot to fit your trading strategy and optimize its performance. Make sure to save the `env` file after making your changes.
