# Bounties

Our bounty program https://harmony.one/bounties is to help the community take part in the development of the Harmony ecosystem.
It covers from core feature to validator tooling, from dApp development to DeFi integration.
Both technical or non-technical bounties can be added.


# Introduction
Anyone can start a bounty in this repo to pay token rewards to those who accomplished the bounty based on the specification.

Each bounty should have a clear definition of the goal, requirement, acceptance criteria, and amount of token rewards.

All the bounties will be listed in the [Issue](https://github.com/harmony-one/bounties/issues) tab.

## How to participate?

You may submit a bounty specification by adding a new `issue`.
Or just be the bounty hunter to finish the bounty based on the spec.

Bounty hunters shall contact the bounty producer directly or comment on the issue for engagement.

A clearly defined acceptance criteria will benefit both producers and hunters to accomplish the bounties.

## Rewards
The reward is usually denoted in the number of Harmony ONE token.

## Examples

Some examples of the potential bounties include large or small, technical or non-technical projects.

- A mobile native wallet of harmony blockchain to support staking
- Another Harmony protocol client implementation, in Rust
- A user guide on how to run, configure a Grafana client to visualize the metrics of Harmony validator

## Links
- Harmony Grant (https://www.harmony.one/grants) Program
# TODO

## Encode Hackathon - Bug Bounty for Harmony Marketplace SDK (Enhancements PR)

As part of the Encode Hackathon, we are offering a bug bounty for the [Harmony Marketplace SDK](https://github.com/blockcoders/harmony-marketplace-sdk) to encourage the community to contribute enhancements and useful additions to the SDK. This bounty is open to developers who are interested in improving the SDK and submitting a pull request (PR) to the repository. Only up to 3 submissions will be accepted.

The goal of this bounty is to improve the usability, functionality, and performance of the Harmony Marketplace SDK. Potential enhancements could include, but are not limited to, adding new features, improving existing functionality, or optimizing the SDK for better performance. The enhancements should be well-documented and clearly explained in the PR.

To qualify for this bounty, contributors must:

1. **Document the enhancements made** to the SDK and comment in this bug bounty issue.
2. **Link to the PR** that is pushed to the Marketplace SDK repository, including the enhancement.
3. **Ensure the PR is accepted** by the maintainers of the SDK.

The reward for this bounty is based on the **enhancements made** and may include **multiple enhancements** bundled together for payment. There are **10 bounties at $50 USD in ONE per bounty**.

### Example Enhancements

Here are some examples of potential enhancements that could be submitted:

- **Add support for new blockchain networks** (e.g., Ethereum, Binance Smart Chain) to the SDK.
- **Implement a new feature** such as token listing, order book, or wallet integration.
- **Improve the SDK's performance** by optimizing API calls or reducing latency.
- **Enhance the SDK's documentation** with detailed examples, usage guides, and API references.
- **Add error handling and logging** to improve the robustness of the SDK.

### Code Example

Below is an example of how you might enhance the SDK by adding a new function to support token listing:

```typescript
// harmony-marketplace-sdk/src/services/marketplace.ts

import { HttpClient } from '@angular/common/http';

export class MarketplaceService {
  constructor(private http: HttpClient) {}

  // New function to list tokens
  listTokens(): Promise<Token[]> {
    return this.http.get<Token[]>('/api/tokens/list').toPromise();
  }
}
```

This example demonstrates how a new function can be added to the SDK to support token listing. The function uses Angular's `HttpClient` to make a request to the `/api/tokens/list` endpoint and returns a promise that resolves to an array of `Token` objects.

By contributing to the Harmony Marketplace SDK, you will not only improve the tooling available to developers but also help promote the Harmony blockchain ecosystem.
