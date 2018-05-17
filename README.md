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

web3.eth.sendTransaction({to: '0x139ccd369d25e251ec59b41363c318fb7257792d', value: web3.toWei(0.00001, 'ether'), data: '0x37284d1ea063dd52b8344a871fbed9f7ef0185153237fad017d8726d448f3780'}, function(a,b){console.log(b)})

ссылка на транзакцию https://rinkeby.etherscan.io/tx/0x7caeb61c13a757f8a0fd093be3a85bcf4488b7857fb2f2130d8f004b7894dd84

### Hard:

## Задание 3

в процессе