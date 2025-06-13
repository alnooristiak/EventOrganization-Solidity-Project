# 🎉 Event Organization Smart Contract | Ethereum DApp (Solidity Project)

A powerful and beginner-friendly **Event Organization Smart Contract** built with **Solidity** for the Ethereum blockchain. This DApp enables decentralized event creation, ticket selling, and ticket transferring — giving both organizers and participants transparency and control.

> ✅ Perfect for your Solidity/Blockchain Developer Portfolio  
> 🚀 SEO-Optimized GitHub Project  
> 💼 Ideal to showcase to recruiters, HRs, and Web3 startups

---

## 🔗 Live Demo (Optional)

**[🔗 View Smart Contract on Remix](https://remix.ethereum.org/)**  
_Deploy and test the contract using MetaMask & Remix._

---

## 🛠️ Tech Stack

- **Solidity** `^0.8.0`
- **Ethereum Blockchain**
- **Remix IDE** / Hardhat / Foundry (Your choice)

---

## 📦 Features

- 📝 **Create Events**: Organizers set event name, future date, ticket price, and ticket quantity
- 🎟️ **Buy Tickets**: Users can buy tickets by sending ETH
- 🔄 **Transfer Tickets**: Users can transfer tickets to other wallet addresses
- ⏳ **Time-based Validation**: Events must be scheduled for the future
- 📉 **Inventory Control**: Prevents overselling and misuse

---

## 🧠 Smart Contract Logic

### ✅ `createEvent(name, date, price, ticketCount)`

- Organizer creates an event.
- Ensures the event date is in the future.
- Ticket count must be greater than 0.

### ✅ `buyTicket(eventId, quantity)`

- Allows attendees to buy tickets for an existing future event.
- Requires correct ETH payment.
- Deducts tickets from remaining supply.

### ✅ `transferTicket(eventId, quantity, to)`

- Users can send their tickets to other addresses.
- Tickets must exist and be valid for a future event.

---

## 🧪 How to Test

You can test the contract using **Remix IDE** or any local Ethereum development environment.

### Example Test Steps:

1. Deploy the contract.
2. Call `createEvent("Web3Conf", 1750000000, 10000000000000000, 100)`  
   (_Date in future, Price = 0.01 ETH_)
3. Call `buyTicket(0, 2)` and send `0.02 ETH`
4. Call `transferTicket(0, 1, 0xReceiverAddress)`

---

## 🔐 Security Notes

- ⛓️ **No access control** — anyone can create events
- ⚠️ **No reentrancy protection** — use with caution in production
- 🛡️ Recommended: Add `Ownable`, `ReentrancyGuard`, and access roles using OpenZeppelin

---

## 💡 Future Improvements

- 🌐 Integrate with a **frontend** (React / Next.js / Ethers.js)
- 🔁 Add **event cancellation & refund** features
- 🎁 Use **Chainlink VRF** for giveaways or raffles
- 🧑‍⚖️ Implement **role-based access** with OpenZeppelin

---

## 🔍 SEO Keywords

`Solidity Event Smart Contract`, `Ethereum DApp Ticketing`, `Blockchain Ticket Sales`,  
`Smart Contract Project`, `Decentralized Event Organizer`, `Web3 Solidity Portfolio`, `Blockchain Developer Project`

---

## 👤 Author

**AL Noor Istiak Mahmud** — Aspiring Smart Contract Developer

- 🔗 [LinkedIn](https://linkedin.com/in/alnooristiak)
- 💻 [GitHub](https://github.com/alnooristiak)
- 🐦 [Twitter](https://twitter.com/alnooristiak)

---

## 🪪 License

This project is licensed under the **Unlicense** — free to use, modify, and distribute.

```solidity
// SPDX-License-Identifier: Unlicense
```
