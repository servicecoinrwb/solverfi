# SolverFi - Decentralized Real-World Asset Financing

![SolverFi Dashboard](https://i.imgur.com/your-dashboard-image-url.png) 

SolverFi is a decentralized finance (DeFi) protocol built on the Arbitrum network, designed to connect stablecoin liquidity providers with real-world businesses seeking short-term invoice financing. The platform allows investors to earn a sustainable, real-world yield on their USDC, while providing businesses with fast, on-chain access to working capital.

---

## 🚀 Key Features

* **For Investors:**
    * **High-Yield Savings:** Deposit USDC into the `InvestorVault` to receive yield-bearing shares.
    * **Real-World Backing:** Yield is generated from interest paid by real-world businesses, not from speculative market activity.
    * **Transparent & On-Chain:** All capital flows, loans, and fee distributions are managed by auditable smart contracts.

* **For Businesses (Solvers):**
    * **Invoice Financing:** Access immediate capital to cover upfront operational costs for service jobs.
    * **Streamlined Repayment:** A simple, two-step process to repay loans after client invoices are paid.

* **For the DAO:**
    * **Complete Admin Dashboard:** A comprehensive UI for managing the entire protocol.
    * **Secure Governance:** Key administrative functions are restricted to the DAO owner, which is intended to be a multi-signature Safe wallet.
    * **Timelocked Controls:** Critical actions, like changing core contract addresses, are protected by a 48-hour timelock to ensure community transparency and security.

---

## 🏛️ System Architecture

The protocol is built on a modular system of smart contracts that work together to manage the flow of capital securely.

1.  **Investor Vault (`InvestorVaultV2`):** The primary capital pool where investors deposit USDC to earn yield.
2.  **Kernel (`KernelSmartAccountV8`):** The operational core of the protocol. It handles the whitelisting of businesses, disburses loans, and processes repayments and fee distributions.
3.  **Yield Vault (`YieldVault`):** A contract that collects the performance fees earned by the protocol, which are controlled by the DAO.

This architecture separates concerns, ensuring that investor funds are handled securely while allowing the DAO to efficiently manage lending operations.

---

## 🏁 Getting Started

This project is a self-contained, single-page application that can be run directly in a web browser.

### Prerequisites

* A web browser with a modern Web3 wallet extension (e.g., MetaMask).
* Your wallet should be connected to the Arbitrum network.

### Running the Dashboard

1.  **Clone the Repository:**
    ```bash
    git clone [https://github.com/servicecoinrwb/solverfi.git](https://github.com/servicecoinrwb/solverfi.git)
    cd solverfi
    ```

2.  **Open the Files:**
    * `landing.html`: The public-facing landing page for the project.
    * `index.html`: The main dashboard dApp for interacting with the smart contracts.
    * `apply.html`: The eligibility form for new businesses.
    * `admin.html`: The internal panel for the DAO to review applications.

    You can open these files directly in your web browser to use the application. All necessary libraries (ethers.js, Tailwind CSS) are loaded via a CDN.
