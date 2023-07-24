# public findings

## 2023-05 USSD

| Severity | Number |
| --- | --- |
| High | 7 |
| Medium | 2 |

### Issues

| title | severity | comments |
| --- | --- | --- |
| [`StableOracleDAI` uses wrong decimals for chainlink feed](https://github.com/sherlock-audit/2023-05-USSD-judging/issues/352) | High | |
| [rebalancing calculates wrong sell amount and can revert](https://github.com/sherlock-audit/2023-05-USSD-judging/issues/351) | High | |
| [removing collateral will lock tokens in contract](https://github.com/sherlock-audit/2023-05-USSD-judging/issues/349) | Medium | |
| [protocol uses uniswap spot price when rebalancing](https://github.com/sherlock-audit/2023-05-USSD-judging/issues/348) | High | |
| [`USSD::mintRebalancer` and `USSD::burnRebalancer` and callable by anyone](https://github.com/sherlock-audit/2023-05-USSD-judging/issues/347) | High | |
| [uniswap trades are done without slippage](https://github.com/sherlock-audit/2023-05-USSD-judging/issues/346) | High | |
| [`StableOracleWBTC` uses wrong price feed](https://github.com/sherlock-audit/2023-05-USSD-judging/issues/345) | High | |
| [Wrong address used for uniswap static oracle](https://github.com/sherlock-audit/2023-05-USSD-judging/issues/344) | High | |
| [no oracle staleness validation](https://github.com/sherlock-audit/2023-05-USSD-judging/issues/343) | Medium | |


## 2023-04 jojo

| Severity | Number |
| --- | --- |
| Medium | 2 |

### Issues

| title | severity | comments |
| --- | --- | --- |
| [unborrowed JUSD are stuck in `JUSDBank`](https://github.com/sherlock-audit/2023-04-jojo-judging/issues/309) | Medium | |
| [`SubAccount::execute` lacks `payable`](https://github.com/sherlock-audit/2023-04-jojo-judging/issues/313) | Medium | |

## 2023-04 Teller (Won contest)

| Severity | Number |
| --- | --- |
| High | 2 |
| Medium | 5 |

### Issues

| title | severity | comments |
| --- | --- | --- |
| [last repayments are calculated incorrectly for "irregular" loan durations](https://github.com/sherlock-audit/2023-03-teller-judging/issues/328) | Medium | in report |
| [due date and defaulting doesn't align](https://github.com/sherlock-audit/2023-03-teller-judging/issues/325) | Medium ||
| [bids can be created against markets that doesn't exist](https://github.com/sherlock-audit/2023-03-teller-judging/issues/323) | Medium | in report |
| [`LenderCommitmentForwarder::updateCommitment` allows lender to be changed](https://github.com/sherlock-audit/2023-03-teller-judging/issues/321) | High | |
| [market owner can front run bids and lower default duration](https://github.com/sherlock-audit/2023-03-teller-judging/issues/320) | Medium | |
| [market owner and protocol can game borrowers](https://github.com/sherlock-audit/2023-03-teller-judging/issues/319) | Medium | |
| [defaulting doesn't change the state of the loan](https://github.com/sherlock-audit/2023-03-teller-judging/issues/317) | Medium | in report |
| [`CollateralManager::commitCollateral` has no access control](https://github.com/sherlock-audit/2023-03-teller-judging/issues/316) | High | |

## 2023-03 Y2K

| Severity | Number |
| --- | --- |
| High | 5 |
| Medium | 2 |

### Issues

| title | severity | comments |
| --- | --- | --- |
| [winnings for an epoch is lost when rolling over](https://github.com/sherlock-audit/2023-03-Y2K-judging/issues/277) | High | | 
| [changing an existing rollover updates the `ownerToRollOverQueueIndex` wrong](https://github.com/sherlock-audit/2023-03-Y2K-judging/issues/278) | High | | 
| [`depositFee` can be bypassed](https://github.com/sherlock-audit/2023-03-Y2K-judging/issues/279) | High | |
| [`Carousel::delistInRollover` can cause positions not to be rolled over](https://github.com/sherlock-audit/2023-03-Y2K-judging/issues/281) | High | |
| [gas costs for minting rollovers is inflated by lost positions](https://github.com/sherlock-audit/2023-03-Y2K-judging/issues/284) | Medium | |
| [emissions for null epochs are lost](https://github.com/sherlock-audit/2023-03-Y2K-judging/issues/285) | Medium | |
| [malicious contract can DoS queues](https://github.com/sherlock-audit/2023-03-Y2K-judging/issues/287) | High | |

## 2023-02 Carapace

| Severity | Number |
| --- | --- |
| High | 3 |
| Medium | 2 |

### Issues

| title | severity | comments |
| --- | --- | --- |
| [a buyer of protection can overprotect their position](https://github.com/sherlock-audit/2023-02-carapace-judging/issues/80) | High | |
| [non claimed `unlockedFunds` are stuck in `ProtectionPool`](https://github.com/sherlock-audit/2023-02-carapace-judging/issues/82) | High | |
| [a protection seller can deposit and withdraw in the same cycle](https://github.com/sherlock-audit/2023-02-carapace-judging/issues/144) | High | |
| [a secondary market for sTokens is dangerous with how withdrawals work](https://github.com/sherlock-audit/2023-02-carapace-judging/issues/146) | Medium | |
| [secondary markets are problematic with how lockCapital works](https://github.com/sherlock-audit/2023-02-carapace-judging/issues/147) | Medium | in report |

## 2023-01 Derby

| Severity | Number |
| --- | --- |
| Medium | 9 |

### Issues

| title | severity | comments |
| --- | --- | --- |
| [vault stakers and game players share the same reward pool](https://github.com/sherlock-audit/2023-01-derby-judging/issues/269) | Medium | in report |
| [multiple withdrawalRequest before the first rebalance will burn LPTokens but only give underlying for the last request](https://github.com/sherlock-audit/2023-01-derby-judging/issues/270) | Medium | |
| [`XChainController::sendFundsToVault` can be griefed and leave `XChainController` in a bad state](https://github.com/sherlock-audit/2023-01-derby-judging/issues/271) | Medium | in report |
| [calling `pushTotalUnderlyingToController` on an inactive vault will break rebalance](https://github.com/sherlock-audit/2023-01-derby-judging/issues/272) | Medium |
| [`Vault::pullFunds` doesn't pull funds from underlying providers correctly](https://github.com/sherlock-audit/2023-01-derby-judging/issues/273) | Medium | in report |
| [allocations to a blacklisted protocol will stop rebalancing](https://github.com/sherlock-audit/2023-01-derby-judging/issues/275) | Medium | |
| [blacklisted protocol still accrues rewards](https://github.com/sherlock-audit/2023-01-derby-judging/issues/302) | Medium | |
| [`Vault::claimTokens` uniswap swaps can be abused](https://github.com/sherlock-audit/2023-01-derby-judging/issues/375) | Medium | |
| [`Swap::swapStableCoins` assumes 1:1 price](https://github.com/sherlock-audit/2023-01-derby-judging/issues/407) | Medium | |

## 2023-01 Popcorn

| Severity | Number |
| --- | --- |
| High | 2 |
| Medium | 4 |

### Issues

| title | severity | comments |
| --- | --- | --- |
| [inital share manipulation attack possible in Vault](https://github.com/code-423n4/2023-01-popcorn-findings/issues/771) | High | |
| [reentrancy in `MultiRewardStaking::claimRewards` for tokens with transfer callbacks, like erc777](https://github.com/code-423n4/2023-01-popcorn-findings/issues/775) | High | |
| [anyone can set fees to 0 after deploy](https://github.com/code-423n4/2023-01-popcorn-findings/issues/777) | Medium | |
| [`Vault::takeFees` can be front run to minimize `accruedPerformanceFee`](https://github.com/code-423n4/2023-01-popcorn-findings/issues/780) | Medium | in report |
| [`takeManagementAndPerformanceFees` calculates fees incorrectly](https://github.com/code-423n4/2023-01-popcorn-findings/issues/784) | Medium | |
| [`quitPeriod` is effectively always just 1 day](https://github.com/code-423n4/2023-01-popcorn-findings/issues/785) | Medium | in report |


## 2023-01 Reserve

| Severity | Number |
| --- | --- |
| Medium | 1 |

### Issues

| title | severity | comments |
| --- | --- | --- |
| [attacker can prevent vesting for a very long time](https://github.com/code-423n4/2023-01-reserve-findings/issues/267) | Medium | in report |

## 2023-01 Ondo

| Severity | Number |
| --- | --- |
| Medium | 1 |

### Issues

| title | severity | comments |
| --- | --- | --- |
| [lack of nonce in kyc signature enables replay](https://github.com/code-423n4/2023-01-ondo-findings/issues/161) | Medium | |


## 2023-01 Biconomy

| Severity | Number |
| --- | --- |
| High | 2 |
| Medium | 2 |

### Issues

| title | severity | comments |
| --- | --- | --- |
| [`tokenGasPriceFactor` can be changed to either maximize gas refund or minimize it](https://github.com/code-423n4/2023-01-biconomy-findings/issues/414) | High | |
| [EIP-1271 contract signing lets anyone execute any tx from the wallet](https://github.com/code-423n4/2023-01-biconomy-findings/issues/382) | High | |
| [`validateUserOp` in `SmartAccount` and `BaseSmartAccount` doesn't follow EIP-4337](https://github.com/code-423n4/2023-01-biconomy-findings/issues/386) | Medium | |
| [methods used by `EntryPoint` has `onlyOwner` modifier](https://github.com/code-423n4/2023-01-biconomy-findings/issues/390) | Medium | in report |


## 2022-12 GoGoPool

| Severity | Number |
| --- | --- |
| High | 2 |
| Medium | 4 |

### Issues

| title | severity | comments |
| --- | --- | --- |
| [any duration can be passed by node operator](https://github.com/code-423n4/2022-12-gogopool-findings/issues/492) | Medium | in report |
| [node operator is getting slashed for full duration even though rewards are distributed based on a 14 day](https://github.com/code-423n4/2022-12-gogopool-findings/issues/493) | High | in report |
| [`recreateMinipool` doesn't require the node operator to have any staked AVAX](https://github.com/code-423n4/2022-12-gogopool-findings/issues/491) | Medium | |
| [slashing fails when node operator doesn't have enough staked `GGP`](https://github.com/code-423n4/2022-12-gogopool-findings/issues/494) | Medium | in report |
| [`finishFailedMinipoolByMultisig` doesn't return staked funds to the node operator](https://github.com/code-423n4/2022-12-gogopool-findings/issues/495) | Medium | |
| [calling `createMiniPool` on an existing minipool in state `Withdrawable` or `Error` locks node operators funds in the vault](https://github.com/code-423n4/2022-12-gogopool-findings/issues/692) | High | |

## 2022-12 Caviar

| Severity | Number |
| --- | --- |
| High | 1 |

### Issues

| title | severity | comments |
| --- | --- | --- |
| [first liquidity provider can make it very expensive for other liquidity providers](https://github.com/code-423n4/2022-12-caviar-findings/issues/249) | High | |


## 2022-12 Forgeries

| Severity | Number |
| --- | --- |
| High | 1 |

### Issues

| title | severity | comments |
| --- | --- | --- |
| [owner can withdraw the NFT at any time if they wait with starting the draw until after `recoverTimelock`](https://github.com/code-423n4/2022-12-forgeries-findings/issues/214) | High | |

## 2022-12 Esher

| Severity | Number |
| --- | --- |
| High | 2 |
| Medium | 1 |

### Issues

| title | severity | comments |
| --- | --- | --- |
| [`saleReceiver` and `feeReceiver` can steal refunds after sale has ended](https://github.com/code-423n4/2022-12-escher-findings/issues/441) | High | in report |
| [wrong configuration can lock `eth` in `LPDA` contract forever](https://github.com/code-423n4/2022-12-escher-findings/issues/442) | High | |
| [seller must sell all NFTs to get paid in `FixedPrice` and `LPDA`](https://github.com/code-423n4/2022-12-escher-findings/issues/443) | Medium | |

## 2022-11 Stakehouse

| Severity | Number |
| --- | --- |
| High | 2 |
| Medium | 1 |

### Issues

| title | severity | comments |
| --- | --- | --- |
| [anyone can steal `eth` from `GiantPools`](https://github.com/code-423n4/2022-11-stakehouse-findings/issues/325) | High | |
| [an early staker in `StakingFundsVault` can take other stakers `eth`](https://github.com/code-423n4/2022-11-stakehouse-findings/issues/387) | High | |
| [`LPTokens` for `StakingFundsVault` can be rotated above max](https://github.com/code-423n4/2022-11-stakehouse-findings/issues/329) | Medium | |

## 2022-10 Inverse (Won contest)

| Severity | Number |
| --- | --- |
| Medium | 4 |

### Issues

| title | severity | comments |
| --- | --- | --- |
| [liquidation is susceptible to oracle price manipulation](https://github.com/code-423n4/2022-10-inverse-findings/issues/424) | Medium | |
| [Oracle uses deprecated chainlink api](https://github.com/code-423n4/2022-10-inverse-findings/issues/435) | Medium | |
| [`Market::repay()` can be DoSed](https://github.com/code-423n4/2022-10-inverse-findings/issues/439) | Medium | |
| [`Market::forceReplenish` can be DoSed](https://github.com/code-423n4/2022-10-inverse-findings/issues/443) | Medium | in report |

## 2022-10 Trader Joe

| Severity | Number |
| --- | --- |
| Medium | 1 |

### Issues

| title | severity | comments |
| --- | --- | --- |
| [Dust trades can keep volatility high](https://github.com/code-423n4/2022-10-traderjoe-findings/issues/436) | Medium | |

## 2022-09 Nouns Builder

| Severity | Number |
| --- | --- |
| Medium | 1 |

### Issues

| title | severity | comments |
| --- | --- | --- |
| [100% founder ownership causes infinite loop in mint](https://github.com/code-423n4/2022-09-nouns-builder-findings/issues/291) | Medium | |

## 2022-08 Olympus DAO


| Severity | Number |
| --- | --- |
| Medium | 1 |

### Issues

| title | severity | comments |
| --- | --- | --- |
| [low market bonds/swaps not working after loan is taken from treasury](https://github.com/code-423n4/2022-08-olympus-findings/issues/422) | Medium | |
