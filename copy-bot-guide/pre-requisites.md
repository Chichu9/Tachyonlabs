---
description: Basic Requirements
---

# Pre-Requisites

### What You Need <a href="#what-you-need" id="what-you-need"></a>

To get started with the Tachyon Copybot, you'll need the following:

1. **Windows or Linux PC**: The Tachyon Copybot is lightweight and can run on an average home PC. For 24/7 operation, consider using a Virtual Private Server (VPS). We do not have a Windows version but you can use Windows WSL to run the program on Windows PC.
2. **Access to a Solana RPC**: An RPC connection is essential for interacting with the Solana blockchain.
3. **Solana Wallet with SOL and WSOL**: SOL is used for gas fees, and WSOL (Wrapped SOL) is used for trades.
4. **Tachyon Copybot File**: The Binary file to run the bot. - Always download the latest version from or discord channel.
5. Licence key to run the bot - You can create a ticket to request your free license key.

### 1. Windows or Linux PC <a href="#id-1.-windows-or-linux-pc" id="id-1.-windows-or-linux-pc"></a>

The Tachyon Copybot is designed to be lightweight, making it suitable for running on most home PCs without significant resource consumption. However, if you want to run the bot continuously, it's advisable to install it on a VPS. VPS options include:

* **Free VPS Options**: Google Cloud and Oracle Cloud offer a free tier for new users, which can be used to run the Tachyon Copybot.
* **Paid VPS Options**: We recommend Hetzner or VULTR.

### 2. Access to a Solana RPC <a href="#id-2.-access-to-a-solana-rpc" id="id-2.-access-to-a-solana-rpc"></a>

An RPC (Remote Procedure Call) connection allows the bot to communicate with the Solana blockchain. Free trials are available from various providers:

* QuickNode
* Helius
* Chainstack
* Syndica
* Solana Vibe Station - We personally recommend SVS RPC, gRPC & VPS.

**Solana Vibe Station** also offers RPC services, and for the best performance, the copybot runs faster using Yellowstone Geyser, which is a high-performance implementation of gRPC designed for Solana. Geyser provides a more efficient way to access blockchain data by streaming updates in real-time, reducing latency and improving the speed of transaction processing.

SVS offers VPS, RPC, and Geyser services within the same data center, ensuring the fastest possible transactions for the copybot. This setup minimizes the time it takes for the bot to receive and act on trading signals, providing a significant advantage in the fast-paced world of crypto trading.

### 3. Solana Wallet with SOL and WSOL <a href="#id-3.-solana-wallet-with-sol-and-wsol" id="id-3.-solana-wallet-with-sol-and-wsol"></a>

The copybot uses SOL for gas fees and WSOL for executing trades. Here’s a brief explanation of each

* **SOL**: The native cryptocurrency of the Solana blockchain, used to pay for transaction fees.
* **wSOL (Wrapped SOL)**: A tokenized version of SOL that can be used in smart contracts and decentralized exchanges.

To convert SOL to WSOL, you can use the Jupiter exchange. This process involves wrapping SOL into WSOL, making it usable for trades within the bot

### 4. Tachyon Copybot Binary <a href="#id-4.-tachyon-copybot-executable" id="id-4.-tachyon-copybot-executable"></a>

The Tachyon Copybot Binary is the program that runs the bot. Below are the instructions for setting it up on Linux, you can follow the same instruction in Windows WSL.

**Linux**

1. Download the Tachyon Copybot executable for Linux.
2. Open a terminal and navigate to the directory where the executable is located.
3. Make the executable file runnable by typing `chmod +x *`.
4. Run the program by typing `./copybot`.
5. On the first run, the program will generate a configuration file named `.env`. This file can be used to configure your settings, including your RPC URL, wallet details, and trading parameters.
6. Configure your `.env` file and run the bot again. It will generate `copy_wallets.txt` and `excluded_wallets.txt`.
