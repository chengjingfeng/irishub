# iriscli gov query-votes

## 描述

查询指定提议的投票情况

## 使用方式

```
iriscli gov query-votes <flags>
```

打印帮助信息:

```
iriscli gov query-votes --help
```

## 标志

| 名称, 速记       | 默认值                      | 描述                                                                                                                                                 | 是否必须  |
| --------------- | -------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- | -------- |
| --proposal-id   |                            | 提议ID                                                                                                        | Yes      |

## 例子

### Query votes

通过指定的提议查询该提议所有投票者的投票详情。

```shell
iriscli gov query-votes --chain-id=<chain-id> --proposal-id=<proposal-id>
```
 
```txt
Votes for Proposal 99:
  iaa1gfcee5u5f54kfcnufv4ypcfyldw0vu0z5l4mh8: Abstain
  iaa15x7ph3pz5dvh92dzhjfcrglswu2r9uygly5vmu: NoWithVeto
```
