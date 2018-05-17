# Неделя 4. Web3 и аудит безопасности

## Задание 1

файл с комментариями по найденным уязвимостям VulnerableOne.sol

## Задание2

### Easy:
var contractAddress = "0xa074e455c2026bf994c2a1c0b0e547f77134d441";

var contract = web3.eth.contract(erc20ABI).at(contractAddress);

contract.balanceOf("0x139CCD369d25E251ec59b41363C318FB7257792D", function(a,b){console.log(b)});

contract.transfer("0x71125a491A736da096c6e0a59229e18eDCA564f2", function(a,b){console.log(b)});

### Medium:
Расчитан хэш sha256 фотки 0x37284d1ea063dd52b8344a871fbed9f7ef0185153237fad017d8726d448f3780 
и записан в блокчейн rinkeby
Чтобы транзакция была выполнена потребовалось "поддать газку" в окошке MetaMask

eth.sendTransaction({from: eth.accounts[0], to: eth.accounts[1], value: web3.toWei(0.00001, 'ether'), data: '0x37284d1ea063dd52b8344a871fbed9f7ef0185153237fad017d8726d448f3780'})

ссылка на транзакцию https://rinkeby.etherscan.io/tx/0x7dca9fa35647aa6b801383c1a986c8978bf00d7a96952bdcfcb4af38cb7fad5e

### Hard:

## Задание 3

в процессе