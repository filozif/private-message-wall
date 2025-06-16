# 🧱 Private Message Wall – Built with Noir

A zero-knowledge based private messaging wall using [Noir](https://noir-lang.org/).  
Messages can be posted and verified without revealing sender identities.

---

## 🧠 Key Features

- ✅ Fully private message commitments using Poseidon hash
- 🧾 Zero-knowledge proof that a message is valid without revealing its content
- 🌐 Designed to be extended into a frontend Aztec SDK dApp

HEAD
### 📬 Contact
Twitter: https://x.com/Milos__Obilic

# 🗳️ Private Voting dApp (on Aztec testnet)

This is a simple **private voting application** powered by **Aztec Protocol** and written in **Noir**.

It allows users to vote anonymously on-chain using zero-knowledge proofs.

## 💡 What it does

- Start an election (admin only)
- Cast a vote secretly (no one can know who voted for whom)
- End the vote and tally results
- All data remains private except final counts

## 🧪 Tech Stack

- 🔐 Aztec Protocol (testnet)
- ⚙️ Noir language
- 🧰 Aztec CLI tools
- 🧪 zk-SNARK based vote validation

## 🚀 How to run

```bash
corepack prepare yarn@4.5.2 --activate
yarn install
yarn build
aztec sandbox
```

## 📂 Project Structure

- `contracts/` – Noir contracts
- `src/` – App logic
- `README.md` – This file
- `yarn-project/` – Aztec SDK logic

## 🧙‍♂️ Why?

To demonstrate how **privacy-first smart contracts** can reshape online governance and DAO elections.

## 🌐 Links

- GitHub: https://github.com/filozif/private-message-wall
- X Profile: https://x.com/Milos__Obilic
>>>>>>> 062976d (Update README with Aztec private voting dApp info)
=======
---

## 📂 Project Structure

```
private-message-wall/
├── src/
│   └── main.nr         # Main contract logic
├── test/
│   └── main.nr         # Test cases using Noir test framework
├── Nargo.toml          # Project configuration
└── README.md
```

---

## 🚀 How to Run (Local Sandbox)

> This project uses Noir and the Aztec sandbox. Follow these steps:

### 1. Clone the Repository
```bash
git clone https://github.com/filozif/private-message-wall
cd private-message-wall
```

### 2. Install Noir
```bash
curl -L https://noirup.sh | sh
nargo --version  # should print version
```

### 3. Build the Circuit
```bash
nargo build
```

### 4. Run the Tests
```bash
nargo test
```

### 5. (Optional) Start Aztec Sandbox in a Separate Terminal
```bash
pnpm cli sandbox --logs
```

---

## 📽️ Demo Video

Check the video below to see how the system works locally.

> **(YouTube/GitHub video link here)**

---

## 🔐 Privacy Mechanism

We use:
- `hash(message, salt)` with Poseidon
- ZK proof to verify commitment
- Public wall stores only `commitments`, not plain messages

---

## 🏗️ Future Ideas

- Frontend: Simple form to submit messages
- Integration with Aztec Connect
- Deploy to Aztec testnet (when available)

---

## 👨‍💻 Author

Created by [@filozif](https://github.com/filozif) for Aztec Dev Bounty  
MIT Licensed
nano README.md
>>>>>>> 006f1b8 (Add final version of README)
