# 董天一

## IPFS: Filecoin 和复制证明

### 概念

- 挑战(challenge): 系统对矿工的提问
- 证明者 (prover): 矿工向系统提供的证明, 完成挑战
- 检验者 (verifier): 系统检测矿工是否完成数据存储任务
- 数据 (data): 用户向矿工提交的需要存储或者已经存储的数据
- 证明 (proof) : 矿工完成挑战是皇后的回答
- 流程: x系统(verifier) 向矿工(prover)发起挑战(chaallenge),矿工答复证明(proof)系统检验矿工的答复以判断是否通过挑战(challenge)


### filecoin 涉及的证明概念

数据持有证明(PDP): 用户发送数据给矿工存储, 矿工证明数据已经被自己存储

可检索证明(PoRet): 和PDP过程类似, 证明矿工存储的数据是可以用来查询

存储证明(Pos): 利用存储空间进行证明, 工作量证明的一种, 性的论文把名称变成了 PoRep

复制证明(Porep): 保证每份数据都说独立存储, 可以防止女巫攻击, 外源攻击和生成攻击

工作量证明(PoW): 证明者向检验者证明自己花费了一定资源, PoW 被用在加密货币, 拜占庭共识和其他各种区块链操作系统. BTC使用的就是这种证明

空间证明(PoSpace): Filecoin 提出的概念, 存储量的证明, PosSpace 是 PoW 的一种, 不同的是 PoW 使用的计算资源, 而 PsSpace 使用的存储资源

时空证明(PoSt): 矿工证明自己花费了 spacetime 资源,即一定时间内存储空间的使用, PoSt 是基于 PoReps 实现

复制证明(PoRep):PoRep 是 PoS 的进化版, 用来证明数据已经被矿工存储

## IPFS 和 Filecoin

P2P协议节点越多, 下载速度越快

IPFS 是一个 P2P 协议

Filecoin 是一个分布式网络, 把云存储变为一个算法市场

没有IPFS, Filecoin 和其他 Storj, sia 一样, 没有区别

Filecoin 和 IPFS 结合在一起, 事情就变得美妙了, filecoin是运行在 ipfs 上的激励层. ipfs 有巨大存储需求, 如果没有奖励机制, 谁愿意贡献如此多的节点和存储呢?

filecoin 可以为 ipfs 提供很多节点, 同时 filecoin 带着一个巨大的分布式存储空间, 解决了 ipfs 存储问题

