personal.unlockAccount(eth.accounts[0],'you4Ever99',1e9)

"C:\Users\ds\AppData\Roaming\Ethereum Wallet\binaries\Geth\unpacked\geth" --rinkeby --fast --verbosity 2 --rpc --rpcport 8547 console

var contractAddress = "0xa074e455c2026bf994c2a1c0b0e547f77134d441"
var contract = web3.eth.contract(erc20ABI).at(contractAddress)
contract.balanceOf("0x139CCD369d25E251ec59b41363C318FB7257792D")
