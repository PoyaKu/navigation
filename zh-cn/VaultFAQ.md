# Golff Vault FAQ常见问题

## 什么是G-HecoToken

G-HecoToken相对Heco版Golff Vault 同等于G-V2Token相对以太版Golff Vault V2，是Golff Vault的权益Token。

## 为什么在机枪池存入1 USDT，得不到1 G-HecoUSDT？

由于Golff机枪池采用的是本金无损策略，目标矿池的收益会由合约自动兑换成本币Token，因持续的收益放入池内，而G-HecoToken的数量不变，用户可凭借G-HecoToken可兑换的Token数量越多。所以Token和G-HecoToken的兑换率并非1:1关系，G-HecoToken是抵押份额权证，每一个G-HecoToken拥有单位净值。
```
单位净值计算公式：单位净值=当前资金池累计Token数量/累计发行G-HecoToken数量
```
当每次收益获取后，单位净值会发生更新。G-HecoUSDT的单位净值为1.1，则您存入10000USDT可以得到：
```
10000 USDT/ 1.1 = 9090.9 G-HecoUSDT
```

## 自动复投及复利机制

自动复投可以简单理解为机枪池会自动将目标池中的收益提取出来并重新投入，以此达到收益复投产生更多收益的机制。由于常规目标收益为固定收益，即投入本金固定，在收益率不变的情况下，收益产出也是固定。而自动复投可以将一定时间的内的收益自动提取出来并重新作为本金投入，以此达到增加收益的目的。

比如若目标固定年化收益率为50%，若按照日进行复投，年化收益率则为：
```
（1+50%/365）^365 -1 = 64.8%
```

我们会发现在复投后，年化收益率会有明显的提升。

## 为何存入后短期内没有收益增加

机枪池收益需要配合Harvest进行收益结算，目前机枪池刚上线，结算触发周期较长，并非实时结算收益，短时间内的存取可能会出现没有收益的情况。所以存入资金后请耐心等待收益结算，即可看到收益变化。