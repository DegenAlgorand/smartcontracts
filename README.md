# smartcontracts
Repository for Degen Smart contracts

## install

Get [Algorand Sandbox](https://github.com/algorand/sandbox)

```
git clone https://github.com/algorand/sandbox.git
cd sandbox
./sandbox up
```

Get Mnemonic from Goal account

```
./sandbox goal account list
./sandbox goal account export -a 47YSI4HIV452ZI2FOOW6IJXAFOSJR6PNJYLAGBQ24CB77GOAYKK5VGCYQE
```

Paste mnemonic info into `algob.config.js`

```
let accounts = mkAccounts([
  {
    // This account is created using `make setup-master-account` command from our
    // `/infrastructure` directory. It already has many ALGOs
    name: "master",
    addr: "47YSI4HIV452ZI2FOOW6IJXAFOSJR6PNJYLAGBQ24CB77GOAYKK5VGCYQE",
    mnemonic:
      "vessel canoe ready couch lunch creek carry wreck swing poet subject man supreme empower train swim mention forest double breeze taste carbon couch above invest",
  },
]);
```
*Install yarn*

Run algob deploy
```
yarn run algob deploy
```