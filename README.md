# Create a repository, and instructions for launching the chain

- To Start Node1 run the following Commands

    ./geth --datadir node1 --unlock "0x1aae10bf1507a3ce67647962B323b3F0AD74F2eD" --mine --rpc --allow-insecure-unlock


- To Start Node2 run the following Commands

    ./geth --datadir node2 --unlock "0x02b1d3b996871F1d75B78fcdDaC6Eef5f64A8473" --mine --port 30304 --bootnodes "enode://bde15f29b82633cbc668ac085ac2fd4c303643f53e166fcac2e93bbfb5362b7c5ec03d11ed2f5669638d4dbd518028c163d4484d88a01c1e2a9873f7b8f66a40@127.0.0.1:30303" --ipcdisable --allow-insecure-unlock

Flags:

- --allow-insecure-unlock:  If you access to a node with geth via HTTP protocol you can´t unlock account with personal.unlockAccount(web3.eth.account, password). If you try, you'll receive error "account unlock with HTTP access is forbidden". So, to avoid that you have to use the flag allow-insecure-unlock.
That is because the unlock operation is unsafe if the node is exposed to external. That "protection" was added in go-ethereum in PR #17037

- --mine allows the node to mine

Configuration:


Explain the configuration of the network, such as it's blocktime, chain ID, account passwords, ports, etc.

- Chain ID: 777
- PWDS:  123
- PORTS:  8454



Explain how to connect MyCrypto to your network and demonstrate (via screenshots and steps) and send a transaction.

![alt text](Screen Shot 2021-04-03 at 12.14.57 AM.png)
![alt text](Screen Shot 2021-04-03 at 12.17.11 AM.png)
![alt text](Screen Shot 2021-04-03 at 12.30.44 AM.png)


Upload the code, including the networkname.json and node folders.
