# iriscli tendermint validator-set

## Description

Get the full tendermint validator set at given height. If no height is specified, the latest height will be used as default.


## Usage

```
  iriscli tendermint validator-set <height> <flags>
```
or
```
  iriscli tendermint validator-set
```

## Flags

| Name, shorthand | Default                    |Description                                                             | Required     |
| --------------- | -------------------------- | --------------------------------------------------------- | -------- |
| --chain-id    |     | Chain ID of Tendermint node   | yes     |
| --node string     |   tcp://localhost:26657                         | Node to connect to |                                     
| --help, -h      |       | 	help for block|    |
| --trust-node    |              true         | Trust connected full node (don't verify proofs for responses)     |          |

## Examples

### Get validator-set at height 114360

```shell
 iriscli tendermint validator-set 114360 --chain-id=<chain-id> --trust-node
```

### Get the latest validator-set

```shell
 iriscli tendermint validator-set --chain-id=<chain-id> --trust-node

```
You will get the following result.

```json
{
  "block_height": "114360",
  "validators": [
    {
      "address": "ica1q9zpqvm7cadx5walcg5jkdxklayr8c2uqtmzmx",
      "pub_key": "icp1zcjduepq8fnuxnceuy4n0fzfc6rvf0spx56waw67lqkrhxwsxgnf8zgk0nus66rkg4",
      "proposer_priority": "-300",
      "voting_power": "100"
    },
    {
      "address": "ica1qxavppd679lyxxu9fdu0zxxfv59r7e0wfgapj7",
      "pub_key": "icp1zcjduepquvkj9qa9mgyhudkhsqxelr0k4zf45ehw4sv4m5wktzhke4zvskas5rk9vq",
      "proposer_priority": "100",
      "voting_power": "100"
    },
    {
      "address": "ica1grd8wp7vezr4czen2nujpejvt6597fmrkqs7h0",
      "pub_key": "icp1zcjduepqnudzfngr6aq4hk47w6p9jx5w97fxmwj2vwwvpkd3sez3dzrm359szchwyl",
      "proposer_priority": "100",
      "voting_power": "100"
    },
    {
      "address": "ica15rg635p4j3xpxcs53dwl6nl2u7gjjsvs7m4psw",
      "pub_key": "icp1zcjduepqxhc5c0fyfwta05tax036jmrr2x6aea2smnce9zhmravt7gwpm0qqjhn9nz",
      "proposer_priority": "100",
      "voting_power": "100"
    }
  ]
}
```





