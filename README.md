<div align="center">

#  👨🏻‍💻 **0G Storage Node Guide** 👨🏻‍💻

</div>


# Device/System Requirements 💻

![image](https://github.com/user-attachments/assets/6f06b201-c4b1-4671-b3e1-bf1e49cb5182)



# Pre-Requirements 🛠

* Add 0G-Galileo-Testnet chain from here: https://docs.0g.ai/run-a-node/testnet-information

* Take faucet: https://faucet.0g.ai/


# Install All Require Dependecies

```
sudo apt-get update && sudo apt-get upgrade -y
```

```
sudo apt install curl iptables build-essential git wget lz4 jq make cmake gcc nano automake autoconf tmux htop nvme-cli libgbm1 pkg-config libssl-dev libleveldb-dev tar clang bsdmainutils ncdu unzip libleveldb-dev screen ufw -y
```

* Install rustup

```
curl https://sh.rustup.rs -sSf | sh
```

```
source $HOME/.cargo/env
```

Check version

```
rustc --version
```


* Install go

```
wget https://go.dev/dl/go1.24.3.linux-amd64.tar.gz && \
sudo rm -rf /usr/local/go && \
sudo tar -C /usr/local -xzf go1.24.3.linux-amd64.tar.gz && \
rm go1.24.3.linux-amd64.tar.gz && \
echo 'export PATH=$PATH:/usr/local/go/bin' >> ~/.bashrc && \
source ~/.bashrc
```

check version

```
go version
```


# Clone the Repository

```
git clone -b v0.8.7 https://github.com/0glabs/0g-storage-node.git
```

```
cd 0g-storage-node
```

* Build in release mode 

```
cargo build --release
```

# Set Configrations





