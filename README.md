# Spheron Network Worker Node
Spheron’s Fizz Nodes offer a low-barrier entry point for anyone looking to contribute resources to Spheron’s decentralized compute network—and earn ongoing rewards for their contributions.

Whether you're looking to run a basic CPU configuration or a powerful GPU setup, this guide will walk you through the entire process

***You earn $FN points that will eventually merge with $SPHN tokens***


# Step-by-Step Guide to Run Fizz Node

## Hardware Requirement
![image](https://github.com/user-attachments/assets/d9d9f0a7-a2f2-41da-8194-16d6dd4b8a00)

## Install Docker
```console
sudo apt update -y && sudo apt upgrade -y
for pkg in docker.io docker-doc docker-compose podman-docker containerd runc; do sudo apt-get remove $pkg; done

sudo apt-get update
sudo apt-get install ca-certificates curl gnupg
sudo install -m 0755 -d /etc/apt/keyrings
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg
sudo chmod a+r /etc/apt/keyrings/docker.gpg

echo \
  "deb [arch="$(dpkg --print-architecture)" signed-by=/etc/apt/keyrings/docker.gpg] https://download.docker.com/linux/ubuntu \
  "$(. /etc/os-release && echo "$VERSION_CODENAME")" stable" | \
  sudo tee /etc/apt/sources.list.d/docker.list > /dev/null

sudo apt update -y && sudo apt upgrade -y

sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin

sudo chmod +x /usr/local/bin/docker-compose

# Docker version check
docker --version
```

## Register Fizz Node
1. Open Your Browser: Navigate to https://fizz.spheron.network
2. Sign up or log in through Gmail or Github
3. Click on the “Register New Fizz Node” Button and Connect your wallet

![image](https://github.com/user-attachments/assets/2876dc7d-dc59-460c-9a0d-f42ce0ea4343)

4. Select your node's OS, resources, Region, Payment Tokens, and Provider ( I selected highest tier provider )

![image](https://github.com/OxcloneNetwork/Spheron_Network/blob/f44829f490b7aa4dfca3e00c744e79a2562a1a72/Screenshot%202025-01-10%20041023.png)

5. Click **“Register Your Fizz Node“**, To complete the registration, you'll need some ETH on the Spheron chain for gas fees. If you don't have any, you can get some from our faucet at https://faucet.spheron.network or Bridge at https://spheron-devnet-eth.bridge.caldera.xyz/

![image](https://github.com/user-attachments/assets/afcd4cd4-240d-46aa-a5d8-6d35bdea0741)

## Run the Fizz Node
1. In setup page for your registered node,Run the Spheron CLI in your terminal then click on the button, generate your token and paste in your terminal.

![image](https://github.com/OxcloneNetwork/Spheron_Network/blob/f44829f490b7aa4dfca3e00c744e79a2562a1a72/Screenshot%202025-01-10%20043115.png)

![image](https://github.com/user-attachments/assets/8c9d5d68-fa8c-42be-96e3-25f9958a0c25)

> You’ll earn more if your node provides higher-tier resources such as a powerful GPU or more CPU cores.

> Fizz Nodes must maintain at least 50% uptime within an ERA (24 hours) to receive rewards

> I've ran this node using CPU-only but you can run with GPU for more rewards

## Check Node health
```
sphnctl fizz logs
```
## To Check Your Node Version
```
sphnctl fizz version
```
## To Stop Your Node 
```
sphnctl fizz stop
```

![image](https://github.com/user-attachments/assets/654ba484-14a2-4994-9a88-bdc10480b327)

Once you've verified the node is running, return to the setup page on the Spheron Fizz App

1. On the setup page, you'll see a "Check Status" button and a switch to "Automatically check status." Click the "Check Status" button to manually initiate a status check for your Fizz node

2. Alternatively, you can toggle on the "Automatically check status" switch to have the system periodically check your node's status without manual intervention

![image](https://github.com/OxcloneNetwork/Spheron_Network/blob/f44829f490b7aa4dfca3e00c744e79a2562a1a72/Screenshot%202025-01-10%20043256.png)

3. The system will now perform checks to validate if your node is active and correctly configured

The validation process may take a few minutes. During this time, the system verifies your node's connectivity, resource availability, and configuration. Once your node is confirmed active, you will be automatically directed to your Fizz dashboard

![image](https://github.com/user-attachments/assets/a35241fd-841b-4ad6-bd99-36dc1a74970c)


## Claim your NFT in the Dashboard

![Screenshot_371](https://github.com/user-attachments/assets/f4b932eb-1ba4-42aa-837e-8d31b36b67f2)


## Join Discord and Claim your role
Discord: https://discord.gg/spheron-network-745315423783878757

Role: https://guild.xyz/spheronfdn

![image](https://github.com/user-attachments/assets/1ffe2ef2-4acc-49df-bc78-b87d7d041f8e)


## Check your VPS resources (RAM, CPU) with htop
```console
# Install htop
sudo apt install htop

# run htop
htop
```
![image](https://github.com/user-attachments/assets/f767070a-543a-4a43-a8d0-8150bfbcf487)
