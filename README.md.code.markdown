# Setup Instructions for Localhost 3000 using npm and Gensyn Testnet

## Initial Setup

```bash
apt update && apt install -y sudo

sudo apt update && sudo apt install -y python3 python3-venv python3-pip curl wget screen git lsof nano unzip iproute2

curl -sSL https://raw.githubusercontent.com/zunxbt/installation/main/node.sh | bash

screen -S gensyn

cd $HOME && rm -rf gensyn-testnet && git clone https://github.com/zunxbt/gensyn-testnet.git && chmod +x gensyn-testnet/gensyn.sh && ./gensyn-testnet/gensyn.sh
```

> **Note:** When you reach the step to select math or hard math, press `ctrl + c`.

## CUDA Installation Steps

```bash
# 1. Update the system
sudo apt-get update
sudo apt-get upgrade

# 2. Download CUDA keyring (from NVIDIA website)
wget https://developer.download.nvidia.com/compute/cuda/repos/ubuntu2204/x86_64/cuda-keyring_1.1-1_all.deb

# 3. Install the keyring with sudo privileges
sudo dpkg -i cuda-keyring_1.1-1_all.deb

# 4. Update apt to recognize the CUDA repository
sudo apt-get update

# 5. Install CUDA
sudo apt-get -y install cuda
```

## Final Step

```bash
cd $HOME && rm -rf gensyn-testnet && git clone https://github.com/zunxbt/gensyn-testnet.git && chmod +x gensyn-testnet/gensyn.sh && ./gensyn-testnet/gensyn.sh
```

---

You can create a GitHub repository, add this `README.md` file, and push it to your remote repo.

---

Nếu bạn cần, tôi có thể hướng dẫn bạn các bước tạo repo, commit và push lên GitHub. Bạn muốn không?