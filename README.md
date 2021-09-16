## sungsu-coin
> 이더리움 기반의 성수 코인 만들기 💰  

### MetaMask 지갑 만들기
- Download Link: https://metamask.io/download.html  
> ![image](https://user-images.githubusercontent.com/20378368/133527549-083c0ad5-7139-40a3-b820-4a0a87d6c489.png)  

### Test Ethereum 얻기
- 5 ETH 제공 💰 약 1시간 소요 😥  
- Faucet Link: https://faucet.dimensions.network/  
> ![image](https://user-images.githubusercontent.com/20378368/133527906-e6eed4d2-9bc7-4e9f-a2c1-63442cbe67f0.png)  

### Remix IDE
- IDE Link: https://remix.ethereum.org/  
> ![image](https://user-images.githubusercontent.com/20378368/133528097-d9f5373e-c4d0-41af-b14d-77f09e4ebc05.png)  
#### Remix IDE: Metadata
```sol
// ----------------------------------------------------------------------------
// Sample token contract
//
// Symbol        : SUNGSU       // 심볼
// Name          : SUNGSU Token // 이름
// Total supply  : 10000000000  // 총 발행량
// Decimals      : 2            // 소수점 자릿수
// Owner Account : 0x5923a3026F5BA4A6F3AaBC01e393fB4ca36456E4   // 계졍의 HEX 주소
//
// Enjoy.
//
// (c) by Idea Inven Doohee 2021. DM Licence.
// ----------------------------------------------------------------------------
```
#### Remix IDE: Constructor
```sol
// ------------------------------------------------------------------------
// Constructor
// ------------------------------------------------------------------------
constructor() public {
    symbol = "SUNGSU";              // 심볼
    name = "SUNGSU Token";          // 이름
    decimals = 2;                   // 소수점 자릿수
    _totalSupply = 10000000000;     // 총 발행량
    balances[0x5923a3026F5BA4A6F3AaBC01e393fB4ca36456E4] = _totalSupply;    // 계졍의 HEX 주소
    emit Transfer(address(0), 0x5923a3026F5BA4A6F3AaBC01e393fB4ca36456E4, _totalSupply);    // 계졍의 HEX 주소
}
```
#### Remix IDE: Compile
> ![image](https://user-images.githubusercontent.com/20378368/133528448-9294e7d5-033e-455f-8a4c-7aa892c3e3f6.png)  
#### Remix IDE: Deploy
> ![image](https://user-images.githubusercontent.com/20378368/133528534-565454d4-5425-4397-917b-6fc61dbfffa9.png)  
> ![image](https://user-images.githubusercontent.com/20378368/133528595-56b4f931-9632-44a0-83dd-600c59be68af.png)  

### Metamask와 연동
- Remix IDE에서 배포된 토큰 계약 주소 복사 > Metamask 계정에 토큰 등록
> ![image](https://user-images.githubusercontent.com/20378368/133529382-b19a11f8-b7de-41b7-9bba-8242c6fd2bdc.png)    
> ![image](https://user-images.githubusercontent.com/20378368/133529031-a3f3d70b-c414-4a51-b4ec-e754e0ed0b58.png)  

### Result
> ![image](https://user-images.githubusercontent.com/20378368/133529268-661a157f-c11d-4de0-bc72-62909c1eadd8.png)  