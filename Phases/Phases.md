
# Phases


<br>

<p align="center">
  <img src=".\image-calum.PNG" width="1280" title="vault use cases" style="page-break-after: avoid;">
</p>
<br>


### Definition

- Staking
    A user allow a smart contracts to hold his/her assets in the hope of collecting them with additional rewards.
- Single-side staking
    Staked assets are comprised of a single token type.
    - example: A user deposit LP tokens to farming pools, to get farming rewards.
    - This rewards amount is proportional to the amount of staked assets and the time duration of staking, and disproportional to the total amount of staked assets.
- Double-side staking
    Staked assets are comprised of two token types.
    - example: A user deposits 1 Eth and 2,000 USDT to Pancakeswap's Eth/USDT pair, to get a share of trading fees.
    - This rewards is proportional to the amount of staked assets, and disproportional to the total amount of staked assets. *It is not necessarily proportional to the time duration of staking.*
    - With the diversity of pool types, like Uniswap v3, which employs the concept of Virtual Liquidity and NLP LP position, it has some more to take into consideration.
- Mult-side staking
    Staked assets are comprised of more than two token types.
    - example: A user deposits 1 Eth, 2,000 USDT, and 0.2 BNB to Balancer's Eth/USDT/BNB pool, to get a share of trading fees.
- Single-token vault
    The vault only handles a single type of staking token.
- Multi-token vault
    The vault handles multiple types of staking token.


### 1st Phase

The 1st phase of the project is to build single-side single-token vaults.
It only existed conceptually.

### 2nd Phase

The 2nd phase of the project is to build single-side multi-token vaults.
The phase is running at the time of writing.

### 3rd Phase

The 3rd phase of the project is to build multi-side multi-token vaults.

## Considerations

### Single-side

- We can deduce an analytical solution of optimal staking portfolio, once the total staked amount is given at any time moment. So we need to predict the total staked amount, if we want a higher profit.


### Double-side, Multi-side

- We can can deduce an analytical solution of optimal staking portfolio, once the total trading volume is given. So we need to predict the total trading volume.