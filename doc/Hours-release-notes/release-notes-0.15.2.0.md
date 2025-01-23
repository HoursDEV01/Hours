## Release Notes: v0.15.2

We are excited to announce the release of v0.15.2, which introduces critical updates, optimizations, and new features to enhance the performance, security, and reliability of the network. Below is a comprehensive summary of the changes in this release and their significance.

### **Key Changes and Features**

#### **1. Activation of Critical Soft Forks (BIP34, BIP65, BIP66, CSV, and SegWit)**
- **BIP34 (Block Height in Coinbase):**
  - Now activated at block height **30200** to enforce inclusion of the block height in the coinbase transaction.
  - Improves chain security and prevents certain forms of replay attacks.
- **BIP65 (CheckLockTimeVerify):**
  - Enforces rules to validate locktimes in transactions, enabling advanced time-based transactions and contracts.
- **BIP66 (Strict DER Signature Encoding):**
  - Ensures signatures follow strict DER encoding, improving transaction validation and preventing malleability attacks.
- **CSV (CheckSequenceVerify):**
  - Enables relative locktime functionality for transactions, allowing creation of advanced multi-step workflows and smart contracts.
- **SegWit (Segregated Witness):**
  - SegWit is fully activated to fix transaction malleability, increase effective block capacity, and reduce transaction fees.

These upgrades enhance the overall security, interoperability, and scalability of the network, bringing it in line with modern blockchain standards.

---

#### **2. New Difficulty Adjustment Algorithm (LWMA)**
- **What is LWMA?**
  - LWMA (Linear Weighted Moving Average) replaces the previous difficulty adjustment algorithm. It calculates the difficulty based on the weighted average of the most recent **94 blocks**, dynamically adjusting the difficulty every block.
- **Advantages:**
  - Faster and smoother difficulty adjustments.
  - Reduced chances of network instability due to sudden hashrate fluctuations.
  - Prevents block-time oscillations, ensuring consistent block production.

This enhancement significantly improves the efficiency and stability of mining operations.

---

#### **3. Enhanced Miner Confirmation Window and Activation Thresholds**
- **New Confirmation Rules:**
  - Updated **activation thresholds** and **confirmation windows** for improved governance and smoother soft fork activations.
  - Default rules:
    - **nRuleChangeActivationThreshold:** 1512 blocks (75%).
    - **nMinerConfirmationWindow:** 2016 blocks.
  - Updated rules for new deployments:
    - **nRuleChangeActivationThresholdV2:** 540 blocks (75%).
    - **nMinerConfirmationWindowV2:** 720 blocks.
- **Why This Matters:**
  - Provides greater flexibility for testing and implementing network upgrades.
  - Ensures activation of new features occurs seamlessly.

---

#### **4. New RPC Commands**
- **`getdifficultyalgorithm`:**
  - Allows users to query the active difficulty adjustment algorithm in real-time.
  - Helpful for miners and node operators to monitor network conditions.

- **`getactivationthresholdinfo`:**
  - Displays the current miner confirmation window and activation thresholds.
  - Essential for understanding when network upgrades or deployments will activate.

These RPC commands enhance transparency and provide better tools for monitoring the network.

---

#### **5. Compatibility Checks for Node Versions**
- Introduced compatibility checks to disconnect peers running incompatible versions of the software after **V152ForkHeight** (30200).
- **Why This Matters:**
  - Prevents network fragmentation by ensuring all connected nodes are running supported versions.
  - Enhances overall network reliability and performance.

---

#### **6. Codebase Improvements**
- Refactored the handling of consensus parameters for better maintainability and flexibility:
  - Unified the height-based activation of soft forks.
  - Simplified future upgrades by consolidating key consensus logic.
- Enhanced logging for debugging and diagnostics:
  - Detailed logs for version mismatches and activation thresholds.
  - Added "DEBUG" logs to track the usage of new consensus rules.

---

### **Benefits of Upgrading to v0.15.2**
1. **Improved Security:**
   - Soft fork activations (BIP34, BIP65, BIP66, CSV, SegWit) significantly enhance the protocol’s resilience against attacks.
2. **Scalability:**
   - SegWit reduces transaction sizes, increases block capacity, and lowers transaction fees.
3. **Mining Efficiency:**
   - LWMA provides faster difficulty adjustments, ensuring smoother block times and better network stability.
4. **Governance:**
   - Updated activation thresholds and confirmation windows provide more flexibility for future upgrades.
5. **Transparency:**
   - New RPC commands allow users to monitor network upgrades and difficulty adjustments in real-time.
6. **Future-Ready:**
   - Refactored consensus handling simplifies the implementation of future network changes.

---

### **Upgrade Instructions**
1. **Backup Your Wallet:**
   - Always back up your wallet.dat file before upgrading.
2. **Download the Latest Release:**
   - [GitHub Repository](https://github.com/HoursDEV01/Hours/releases/tag/v0.15.2).
3. **Stop Running Nodes:**
   - Shut down any running instances of the wallet or node before upgrading.
4. **Install the New Version:**
   - Follow the installation instructions for your operating system.
5. **Restart and Resync:**
   - Allow the wallet or node to resync with the blockchain to ensure all changes are applied.

---

### **Conclusion**
Version v0.15.2 marks a significant milestone in the network’s evolution, bringing critical upgrades and modern features to improve performance, security, and scalability. We encourage all users, miners, and node operators to upgrade as soon as possible to take full advantage of these enhancements and support the network’s continued growth.

Thank you for your support and contributions!

