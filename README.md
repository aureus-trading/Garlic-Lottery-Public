# Garlic-Lottery-Public

Lucky Cloves, a Decentralized Garlicoin Lottery

How does it work?
You visit https://lucky.garlicoin.io/ and press start game. 
Then you get a game key. (This key can be used to access your game with your deposited grlc in it.) 
Once you deposit GRLC you can start playing.

The odds are the following:
Bread: 6.9% => after 14.49 spins you should win
Butter: 0.69% => after 144.92 spins you should win
Garlic: 0.069% => after 1449.27 spins you should win

The prizes are:
3 x Bread: 5 GRLC
3 x Butter: 69 GRLC
3 x Garlic: Jackpot (currently 2278 GRLC)

What happens with the 1 GRLC i pay per spin?
0.997 GRLC goes into the jackpot which you can see here: https://explorer.turtlenetwork.eu/address/3JqHSKjiDGNXCHc1LL1QHeQa6t11dMHVbnH/assets

0.003 GRLC pays the transaction fees and executes the lottery dapp.

Only 69% gets paid out for 3 x Garlic, this is why the game shows only 69% of this.
The rest is then used for the next jackpot. So then the game can go on without ever going to zero.



How is it built?
The dapp was built in collaboration with Polarity.Exchange. Similar to wrapped GRLC on BSC and ETH, our first wrapped version was actually on Turtle.Network (TN) which polarity.exchange is built on. The math behind the lottery is a smart contract on TN. Behind the curtains you wrap your GRLC to play the slot machine. (Garlic Lottery Contract)

The whole project is open sourced (LINK TO GITHUB) and can be used to make your own dapps.

To edit smart contracts for Turtle.Network you can use the IDE from here: https://waves-ide.com/ using the following custom network settings in the top right:

1.2. 

https://github.com/wavesplatform/ride-introduction ( Learning about RIDE ( Contracts on TN/Waves )
https://stepik.org/course/54415/promo - Full Smart Contract Course ( FREE )

Why use RIDE smart contracts?
The language RIDE is what is known as a “non turing complete” language, whereas Solidity ( used on ETH ) is “turing complete”. This means that RIDE lacks a high degree of complexity and some processes cannot be 100% automated on chain. The strength you inherit from giving up the complexity is a heightened level of security. The only concerns you will have in programming for RIDE is ensuring that you have set your permissions properly for your functions. Users will not be able to overflow integers, nor will they be able to run any re entrancy exploits. On the TN chain there is no front running, all transactions are processed with equal priority into micro blocks during an instant state change. 

Because GRLC is a “sponsored asset” on the TN chain, users can use GRLC as gas on the platform for all operations. GRLC can be the main currency in dApps, it can also be the gas users pay to the network. Leveraging the TN chain will allow you to build flexible dApps and decentralized frameworks for GRLC while also having exposure to a wide variety of assets to trade against thanks to Polarity.Exchange.
