# Solana Raydium Volume Bot

Designed to automate the distribution of SOL to multiple wallets and execute endless buy and sell swap transactions simultaneously on the Raydium and Meteora platform. It leverages Solana's blockchain technology to perform these operations efficiently.
And add feature to boost volume in Marketplace, real-time Volume Monitoring, automated Execution, integration with Raydium and Solana and customizable strategies. Analyze trading volume and price movements to make decisions about when to buy or sell assets.

# 👋 Contact Me

### 
Telegram: https://t.me/earthzeta
###
<div style={{display : flex ; justify-content : space-evenly}}> 
    <a href="https://discordapp.com/users/339619501081362432" target="_blank"><img alt="Discord"
        src="https://img.shields.io/badge/Discord-7289DA?style=for-the-badge&logo=discord&logoColor=white"/></a>
    <a href="https://t.me/earthzeta" target="_blank"><img alt="Telegram"
        src="https://img.shields.io/badge/Telegram-26A5E4?style=for-the-badge&logo=telegram&logoColor=white"/></a>
</div>


#### Feel free to contact me if you need any help.

# Overview

### What is the main difference between the former volume booster and the updated one?

## 🔧 Last Version's Demerits
- ❌ **Repetitive buy and sell with one wallet**: The last version of the Raydium Volume Bot used fixed wallets, so it was apparent on DexScreener that some wallets performed repetitive buy and sell actions.
- ❌ **No increase in the number of holders**: It didn't increase the number of holders, only the volume.
- ❌ **Gathering token instead of SOL**: When gathering, if there were tokens left, it didn't sell them before gathering. Instead, it just gathered tokens to the main wallet.
- ❌ **Equal number of buys and sells**: One-time buy and one-time sell actions left sell pressure at the end, as there was always a sell at the end of the volume operation.

## 🚀 Improvements
- ✅ **Transferring SOL to new wallet**: After buying and selling in one wallet, it transfers SOL to a newly created wallet and continues buying and selling there.
- ✅ **Holder increase**: New wallets are created every round of buying and selling, increasing the number of holders.
- ✅ **Sell before gather**: When gathering, if there are tokens left in the wallet, it sells the tokens first and gathers only SOL (the token account rent of 0.00203 SOL is reclaimed).
- ✅ **More buys than sells**: It randomly buys twice with SOL in the wallet and sells all tokens after some time, making the number of buys twice as many as sells, thus creating more buy pressure.

## 🌟 Features
- ⚙️ **Automated SOL Distribution**: Distributes SOL to new wallets.
- 🔄 **Endless Buy and Sell Swaps**: Performs simultaneous buy and sell transactions.
- 🚀 **Swap with Jupiter V6**: Swap is performed with Jupiter V6 swap aggregator.
- 🚀 **Swap with Meteora SDK: Swap is performed with Meteora dlmm and dyn SDK.
- 🛠️ **Configurable Parameters**: Allows customization of buy amounts, intervals, distribution settings, and more.

## Example
https://solscan.io/account/EqCgCTBSSqdzaZDr6r1LPsysXdJwc2jn3CBqD5dNQS6Q

https://github.com/user-attachments/assets/df532c73-3c68-42e7-828a-4e1927c42047



#  🚀 Usage
### 1. Clone the repository
```
git clone https://github.com/earthzetaorg/solana-raydium-volume-bot.git
cd solana-raydium-volume-bot
```
### 2. Install dependencies
```
npm install
```
### 3. Configure the environment variables

Rename the .env.copy file to .env and set RPC and WSS, main keypair's secret key and other variables.

### 4. Run the bot

```
npm start
```

### 5. Gather the funds from distributed wallets

```
npm run gather
```


