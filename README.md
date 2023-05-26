# public findings

## 2023-03 Y2K

### winnings for an epoch is lost when rolling over
High
- https://github.com/sherlock-audit/2023-03-Y2K-judging/issues/277

### changing an existing rollover updates the `ownerToRollOverQueueIndex` wrong
High
- https://github.com/sherlock-audit/2023-03-Y2K-judging/issues/278

### `depositFee` can be bypassed
High
- https://github.com/sherlock-audit/2023-03-Y2K-judging/issues/279

### executed rollovers can be delisted which trades places with last unexecuted one
High
- https://github.com/sherlock-audit/2023-03-Y2K-judging/issues/280

### `Carousel::delistInRollover` can cause positions not to be rolled over
High
- https://github.com/sherlock-audit/2023-03-Y2K-judging/issues/281

### gas costs for minting rollovers is inflated by lost positions
Medium
- https://github.com/sherlock-audit/2023-03-Y2K-judging/issues/284

### emissions for null epochs are lost
Medium
- https://github.com/sherlock-audit/2023-03-Y2K-judging/issues/285

### malicious contract can DoS queues
High
- https://github.com/sherlock-audit/2023-03-Y2K-judging/issues/287

### malicious contract can make minting queued items very expensive
High
- https://github.com/sherlock-audit/2023-03-Y2K-judging/issues/288

## 2023-02 Carapace

### a buyer of protection can overprotect their position
High
- https://github.com/sherlock-audit/2023-02-carapace-judging/issues/80

### non claimed `unlockedFunds` are stuck in `ProtectionPool`
High
- https://github.com/sherlock-audit/2023-02-carapace-judging/issues/82

### a protection seller can deposit and withdraw in the same cycle
High
- https://github.com/sherlock-audit/2023-02-carapace-judging/issues/144

### a secondary market for sTokens is dangerous with how withdrawals work
Medium
- https://github.com/sherlock-audit/2023-02-carapace-judging/issues/146

### secondary markets are problematic with how lockCapital works
Medium, in report
- https://github.com/sherlock-audit/2023-02-carapace-judging/issues/147

## 2023-01 Derby

### vault stakers and game players share the same reward pool
Medium, in report
- https://github.com/sherlock-audit/2023-01-derby-judging/issues/269

### multiple withdrawalRequest before the first rebalance will burn LPTokens but only give underlying for the last request
- https://github.com/sherlock-audit/2023-01-derby-judging/issues/270

### `XChainController::sendFundsToVault` can be griefed and leave `XChainController` in a bad state
Medium, in report
- https://github.com/sherlock-audit/2023-01-derby-judging/issues/271

### calling `pushTotalUnderlyingToController` on an inactive vault will break rebalance
Medium
- https://github.com/sherlock-audit/2023-01-derby-judging/issues/272

### `Vault::pullFunds` doesn't pull funds from underlying providers correctly
Medium, in report
- https://github.com/sherlock-audit/2023-01-derby-judging/issues/273

### allocations to a blacklisted protocol will stop rebalancing
Medium
- https://github.com/sherlock-audit/2023-01-derby-judging/issues/275

### blacklisted protocol still accrues rewards
Medium
- https://github.com/sherlock-audit/2023-01-derby-judging/issues/302

### `Vault::claimTokens` uniswap swaps can be abused
Medium
- https://github.com/sherlock-audit/2023-01-derby-judging/issues/375

### `Swap::swapStableCoins` assumes 1:1 price
Medium
- https://github.com/sherlock-audit/2023-01-derby-judging/issues/407

## 2023-01 Popcorn

### inital share manipulation attack possible in Vault
High
- https://github.com/code-423n4/2023-01-popcorn-findings/issues/771

### reentrancy in `MultiRewardStaking::claimRewards` for tokens with transfer callbacks, like erc777
High
- https://github.com/code-423n4/2023-01-popcorn-findings/issues/775

### anyone can set fees to 0 after deploy
- https://github.com/code-423n4/2023-01-popcorn-findings/issues/777

### `Vault::takeFees` can be front run to minimize `accruedPerformanceFee`
Medium, in report
- https://github.com/code-423n4/2023-01-popcorn-findings/issues/780

### `takeManagementAndPerformanceFees` calculates fees incorrectly
Medium
- https://github.com/code-423n4/2023-01-popcorn-findings/issues/784

### `quitPeriod` is effectively always just 1 day
Medium, in report
- https://github.com/code-423n4/2023-01-popcorn-findings/issues/785

## 2023-01 Reserve

### attacker can prevent vesting for a very long time
Medium, in report
- https://github.com/code-423n4/2023-01-reserve-findings/issues/267

## 2023-01 Ondo

### lack of nonce in kyc signature enables replay
Medium
- https://github.com/code-423n4/2023-01-ondo-findings/issues/161

## 2023-01 Biconomy

### `tokenGasPriceFactor` can be changed to either maximize gas refund or minimize it
High
- https://github.com/code-423n4/2023-01-biconomy-findings/issues/414

### EIP-1271 contract signing lets anyone execute any tx from the wallet
High
- https://github.com/code-423n4/2023-01-biconomy-findings/issues/382

### `validateUserOp` in `SmartAccount` and `BaseSmartAccount` doesn't follow EIP-4337
Medium
- https://github.com/code-423n4/2023-01-biconomy-findings/issues/386

### methods used by `EntryPoint` has `onlyOwner` modifier
Medium, in report
- https://github.com/code-423n4/2023-01-biconomy-findings/issues/390

## 2022-12 GoGoPool

### any duration can be passed by node operator
Medium, in report
- https://github.com/code-423n4/2022-12-gogopool-findings/issues/492

### node operator is getting slashed for full duration even though rewards are distributed based on a 14 day cycle
High, in report
- https://github.com/code-423n4/2022-12-gogopool-findings/issues/493

### `recreateMinipool` doesn't require the node operator to have any staked AVAX
Medium
- https://github.com/code-423n4/2022-12-gogopool-findings/issues/491

### slashing fails when node operator doesn't have enough staked `GGP`
Medium, in report
- https://github.com/code-423n4/2022-12-gogopool-findings/issues/494

### `finishFailedMinipoolByMultisig` doesn't return staked funds to the node operator
Medium
- https://github.com/code-423n4/2022-12-gogopool-findings/issues/495

### calling `createMiniPool` on an existing minipool in state `Withdrawable` or `Error` locks node operators funds in the vault
High
- https://github.com/code-423n4/2022-12-gogopool-findings/issues/692

## 2022-12 Caviar

### first liquidity provider can make it very expensive for other liquidity providers
High
- https://github.com/code-423n4/2022-12-caviar-findings/issues/249

## 2022-12 Forgeries

### owner can withdraw the NFT at any time if they wait with starting the draw until after `recoverTimelock`
High
- https://github.com/code-423n4/2022-12-forgeries-findings/issues/214

## 2022-12 Esher

### `saleReceiver` and `feeReceiver` can steal refunds after sale has ended
High, in report
- https://github.com/code-423n4/2022-12-escher-findings/issues/441

### wrong configuration can lock `eth` in `LPDA` contract forever
High
- https://github.com/code-423n4/2022-12-escher-findings/issues/442

### seller must sell all NFTs to get paid in `FixedPrice` and `LPDA`
Medium
- https://github.com/code-423n4/2022-12-escher-findings/issues/443

## 2022-11 Stakehouse

### anyone can steal `eth` from `GiantPools`
High
- https://github.com/code-423n4/2022-11-stakehouse-findings/issues/325

### an early staker in `StakingFundsVault` can take other stakers `eth`
High
- https://github.com/code-423n4/2022-11-stakehouse-findings/issues/387

### `LPTokens` for `StakingFundsVault` can be rotated above max
Medium
- https://github.com/code-423n4/2022-11-stakehouse-findings/issues/329

## 2022-10 Inverse

### liquidation is susceptible to oracle price manipulation
Medium
- https://github.com/code-423n4/2022-10-inverse-findings/issues/424

### Oracle uses deprecated chainlink api
Medium
- https://github.com/code-423n4/2022-10-inverse-findings/issues/435

### `Market::repay()` can be DoSed
Medium
- https://github.com/code-423n4/2022-10-inverse-findings/issues/439

### `Market::forceReplenish` can be DoSed
Medium, in report
- https://github.com/code-423n4/2022-10-inverse-findings/issues/443

## 2022-10 Trader Joe

### Dust trades can keep volatility high
Medium
- https://github.com/code-423n4/2022-10-traderjoe-findings/issues/436

## 2022-09 Nouns Builder

### 100% founder ownership causes infinite loop in mint
Medium
- https://github.com/code-423n4/2022-09-nouns-builder-findings/issues/291

## 2022-08 Olympus DAO

### low market bonds/swaps not working after loan is taken from treasury
Medium
- https://github.com/code-423n4/2022-08-olympus-findings/issues/422