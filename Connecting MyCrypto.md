# Transacting on your chain

In this activity, you will be connecting MyCrypto to your custom chain, importing your pre-funded wallet, then sending a test transaction to yourself!

## Instructions

First, you will need to get the private key of your pre-funded address and keep it handy for later.

* Open up MyCrypto to get the private key of the ETH address you used to pre-fund your chain. Be sure the `Kovan` network is selected.

 ![Verify Kovan network](screenshots/verify-kovan.gif)

* Unlock your wallet using your mnemonic phrase and choose the address you want to inspect.

* Select the ETH address you used to pre-fund your chain, and in the "Select" dropdown list, choose `Wallet Info`.

* Click on the eye icon next to the `Private Key` field, and copy and paste the private key of the wallet. Keep this handy, as you will use it in a bit.

 ![Get private key](screenshots/get-private-key.gif)

Now you are going to connect MyCrypto with the blockchain you created. Follow the next steps.

* Open up MyCrypto, then click `Change Network` at the bottom left:

 ![change network](screenshots/change-network.png)

* **NOTE:** Changing networks will automatically clear your loaded wallet, so make sure your private key has been stored in your notes for use in the next steps. 

* Click "Add Custom Node", then add the custom network information that you set in the genesis.

* Make sure that you scroll down to choose `Custom` in the "Network" column to reveal more options like `Chain ID`:

 ![custom network](screenshots/custom-network.png)

* The chain ID must match what you came up with earlier.

* The URL must point to the default RPC port on your local machine. Use `http://127.0.0.1:8545`.

* Once you save and use the network, double-check that it is selected and is connected.

Now that you are connected to your blockchain, you will need to load the private key you created and funded on the network.

* On the left pane menu, click on "View & Send".

* Next, click on the "Private Key" option to continue.

 ![Open wallet step 1](screenshots/open-wallet-1.png)

* A new window will pop-up. Paste the private key of the pre-funded wallet and click on the "Unlock" button to continue.

 ![Open wallet step 2](screenshots/open-wallet-2.png)

* Looks like we're filthy rich! This is the balance that was pre-funded for this account in the genesis configuration; however, these millions of ETH tokens are just for testing purposes.

 ![prefunded account](screenshots/prefunded-account.png)

Now we're going to send a transaction to ourselves to test it out. Follow the next steps.

* Copy the pre-funded address into the "To Address" field, then fill in an arbitrary amount of ETH:

 ![transaction send](screenshots/transaction-send.png)

* Confirm the transaction by clicking "Send Transaction", and the "Send" button in the pop-up window.

 ![Send transaction](screenshots/send-transaction.gif)

* Click the `Check TX Status` when the green message pops up, then confirm the logout:

 ![check tx](screenshots/check-tx-status.png)

* You should see the transaction go from `Pending` to `Successful` in around the same block time you set in the genesis.

* You can click the `Check TX Status` button to update the status.

 ![successful transaction](screenshots/transaction-status.png)

Congratulations! That was the first transaction sent on this blockchain network!

---

© All images are copied from gitlab Activities