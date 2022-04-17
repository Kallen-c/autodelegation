![](https://i.yapx.ru/RTuEU.jpg)

___In this guide, we have written how to set up an autodelegator for your validator node. The guide is suitable for any project of the cosmos network___

We need to do is set the variables correctly
```html
curl -s https://raw.githubusercontent.com/Kallen-c/autodelegation/main/autodelegator > autodelegator.sh && chmod +x autodelegator.sh && ./autodelegator.sh
```
1. The name of the project corresponds to the node startup service file
__Project example - evmos__

2. The name of the wallet that you wrote when installing the node
3. The password is set according to your password from the created wallet
4. The validator address and the delegator address will be set automatically, the only thing you need to do is enter the wallet password when setting the variable
5. You can find out the DENOM variable when requesting the balance of tokens on your wallet, this will be the name of the coins
6. The FEES variable is usually set to 0, but depends on the network
7. CHAIN ​​ID is usually set by the name of the testnet or mainnet
__Chain id example - evmos_9001-1__

**After you have set the variables, go to the launch of the redelegator**

The script will automatically open the screen window, where all you have to do is run the redelegator with the command
```html
cd $HOME/autodelegate && ./start.sh
```
and exit the window by pressing

__ctrl + a + d__

in order to go back to the window

__screen-r__
