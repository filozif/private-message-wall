# 🧱 Private Message Wall – Built with Noir

A zero-knowledge based private messaging wall using [Noir](https://noir-lang.org/).  
Messages can be posted and verified without revealing sender identities.

---

## 🧠 Key Features

- ✅ Fully private message commitments using Poseidon hash
- 🧾 Zero-knowledge proof that a message is valid without revealing its content
- 🌐 Designed to be extended into a frontend Aztec SDK dApp

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

> ✅ Last updated and tested on **17 June 2025** using **Aztec SDK v0.87.8**.  
> All tests pass and the project works end-to-end with the latest Aztec sandbox and CLI.

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
