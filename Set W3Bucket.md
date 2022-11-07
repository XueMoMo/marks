# Set W3Bucket

# 1.设置容量和可铸造数量

调用setBucketEditions方法设置。

**注意：每次设置后，之前设置的都将作废。**

参数说明：

editions： 二维数组类型，表示多种容量， 例如

```js
// [editionId(1<=editionId<=100), 容量(GB), 可mint数量(<=1000000)]
// editionId=1,容量1TB,mintSupply=1000000 和 editionId=2,容量10TB,mintSupply=1000000
[[1,1024,1000000],[2,10240,1000000]]
```

示例截图：

![](https://gw-seattle.cloud3.cc/ipfs/QmdNcyHJoFz1gxemdk8BnpTKEcYmGP8YJpkztPMGs5sAiP)

# 2.设置价格

调用setBucketEditionPrices方法

**注意1：设置将覆盖之前的价格**

**注意2：小数点位数，ETH 18位， USDT 6位 。也可以添加任何ERC20的代币。**

参数说明：

editionId： 数字类型 ， 例如 1 , 应使用上一步中的 editionId

prices： 二维数组类型，表示多种价格， 例如  

```js
  //表示 1 ETH
 [['0x0000000000000000000000000000000000000000','1000000000000000000']]
 // 表示 1 USDT
 [['0xdAC17F958D2ee523a2206206994597C13D831ec7','1000000']] 
  // 表示 1 ETH or 1 USDT
 [['0x0000000000000000000000000000000000000000','1000000000000000000'],['0xdAC17F958D2ee523a2206206994597C13D831ec7','1000000']]
```

    截图示例：

![](https://gw-seattle.cloud3.cc/ipfs/QmbmdLo856zy4RNYaKsYudM7PcsXR81Hv1hFTxf83NEB7a)
