# dWallet
### Step 1: System Requirements
Ensure your machine meets the following minimal requirements:
- **OS**: Ubuntu 20.04 or later
- **CPU**: 4+ cores
- **RAM**: 8GB+
- **Storage**: 100GB SSD
- **Network**: High-speed internet with open ports for peer-to-peer communication.

### Step 2: Install Dependencies
You will need to install the following dependencies:
- **Git**: `$ sudo apt-get install git`
- **Docker**: `$ sudo apt-get install docker.io`
- **Rust** (for compiling code): `$ curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh`

### Step 3: Clone the dWallet Network Repository
Fork the official dWallet repository from GitHub and clone it locally:
```bash
git clone https://github.com/dwallet-network/dwallet-network.git
cd dwallet-network
```

### Step 4: Build and Install dWallet
Navigate to the directory and compile the dWallet software:
```bash
cargo build --release
```
This will install the necessary binaries for running a validator node.

### Step 5: Initialize Your Validator Node
Configure the node to operate on the dWallet testnet:
```bash
./dwallet init --chain testnet
```

### Step 6: Generate Validator Keys
You'll need to create a keypair to identify your validator:
```bash
./dwallet keys generate
```
Store your key information securely.

### Step 7: Start the Validator Node
Once configured, you can start your node by running:
```bash
./dwallet start --validator --chain testnet
```

### Step 8: Monitor and Maintain
You can monitor your node's performance through log outputs and use CLI commands for status checks and maintenance.
