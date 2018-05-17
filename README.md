# Неделя 4. Web3 и аудит безопасности

## Задание 1

файл с комментариями по найденным уязвимостям VulnerableOne.sol

## Задание2

### Easy:
var contractAddress = "0xa074e455c2026bf994c2a1c0b0e547f77134d441"
var contract = web3.eth.contract(erc20ABI).at(contractAddress)
contract.balanceOf("0x139CCD369d25E251ec59b41363C318FB7257792D", function(a,b){console.log(b)});

### Medium:

### Hard:

## Задание 3