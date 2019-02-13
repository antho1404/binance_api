# binance_api
Mesg service for Binance API

```bash
mesg-core service deploy https://github.com/joveeee/binance_api
```

## Tasks

### Get coin price change 

Task key: **getCoinPriceChange**


#### Inputs

| **key** | **type** | **description** |
| --- | --- | --- |
| **coinpair** | `String` | Coin pair ( for example - LTCBTC )  |
| **interval** | `String` | 1h, 1m, 24h etc (see [binance](https://www.binance.com/en) exchange) |
| **intervalNum** | `String` | How many intervals to take (if interval 1 and intervalNum2, we get price change for last 2 hour separately)  |


#### Outputs

##### error

Output key: **error**

Return a `error` with the error message

| **key** | **type** | **description** |
| --- | --- | --- |
| **error** | `String` |  |

##### success

Output key: **success**

Return the array of tweet object ( tweet object inluce a lot of data, see Twitter API)

| **key** | **type** | **description** |
| --- | --- | --- |
| **message** | `String ` |  | |
| **priceChange** | `Array of number ( price changes ) ` |  | |



