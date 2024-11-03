# FAQ (Frequently Asked Questions)

**1. Is it safe to use Copybot and put my wallet private key?**

**Yes, it is safe.** The private key stays on your computer and is not sent outside or stored on any server, making it even safer than using Telegram bots. Always ensure you download Tachyon Copybot from official sources. Never use Tachyon Copybot or any other bots without proper vetting, as malicious code can drain your wallet.

**2. I have never used a CLI bot before. Please help me.**

If you need help, please join our Discord server. You can chat with other users for assistance or open a ticket, and a staff member will help you. [https://discord.gg/](https://discord.gg/tachnode)[tachyon](../)

**3. Why are my transactions slow?**

There are several reasons why your transactions may be slow:

* **Jito Tip**: The tip you provide to prioritize your transactions.
* **Latency**: The time it takes for your computer to communicate with the RPC.
* **Use of gRPC**: Utilizing gRPC (Geyser) can speed up transactions.
* **Competition**: High demand for the token you're trading.
* **Solana Congestion**: Network congestion can slow down transactions.

For the fastest transactions, consider subscribing to TachNode. Our VPS/RPC/gRPC combo in the same data center, close to the Jito block engine, provides the best setup for speedy transactions.

**4. What is a VPS?**

A **Virtual Private Server (VPS)** is a virtual machine provided by a hosting service. It runs its own copy of an operating system, and customers have superuser-level access to that operating system instance. This allows them to install almost any software that runs on that OS.

**5. What is an RPC?**

**Remote Procedure Call (RPC)** is a protocol used by the bot to communicate with the Solana blockchain. It allows the bot to send transactions and retrieve blockchain data.

**6. I cannot afford a VPS!**

There are free options like Google Cloud and Oracle Cloud that offer a free tier. Additionally, the bot can run on your home PC if you can't afford a VPS.

**7. I cannot afford RPC!**

Some free RPC options are available:

* QuickNode
* Helius
* Chainstack
* Syndica

**8. How much quote size should I use?**

We recommend starting small at 1% of your funds. If you have 1 SOL, use 0.01 SOL as the quote size. You can increase the amount once you see consistent returns.

**9. What is a Jito Tip?**

We have an automatic optimal Jito tip. It is recommended to start at the 75th percentile for the best balance between landing speed and cost.

**10. How to find copy wallets?**

We recommend reading our guide on finding and selecting copy wallets.

**11. Why do I see nonce transactions on Solscan?**

Copybot uses **durable nonces** to sign all transactions. This method provides benefits such as ensuring that transactions can be retried without being invalidated due to nonce conflicts, enhancing reliability.

**12. I lost all my money!**

Trading crypto involves significant risks. To minimize risk from copy trading, consider these strategies:

* **Check the Copywallet Guide**: Follow our guide to choose reliable wallets to copy.
* **Ask for Help**: Join the TachNode Discord community for support and advice.
* **Diversify**: Copy multiple wallets to spread your risk.
* **Start Small**: Begin with a small quote size and increase as you gain confidence and see consistent returns.
