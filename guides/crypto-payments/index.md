---
title: Send and Receive Crypto Payments
description: This page gives an overview of the crypto payments feature.
---

## Overview

Unstoppable Domains allows you to make payments with over [281 cryptocurrencies](https://support.unstoppabledomains.com/support/solutions/articles/48001185621-what-cryptocurrencies-are-currently-supported-) using a single domain name. As long as you have configured your addresses to the domain, users can send crypto to your domain, and it will end up in your wallet.

Still confused about how it works? If you own the `ryan.crypto` domain and a user sends BTC to that domain, you will receive it at your BTC address. If another user sends ETH to that domain, you will receive it at your ETH address.

> Unstoppable Domains achieves this with a process called domain resolution.

![success payment example](../../images/success-payment-example.gif)

## What is Domain Resolution?

Domain resolution is the process of converting a human-readable domain name like `ryan.crypto` to the cryptocurrency addresses attached to them. It involves retrieving a domain’s records through smart contracts deployed on the blockchain.

![domain resolving example](../../images/best-practices.png)

## How is a Domain Resolved?

In the demo above, we sent 1 `ETH` to the `ryan.crypto` domain. The application sends both parameters (currency and domain) to the [Resolver contract](https://docs.unstoppabledomains.com/domain-registry-essentials/cns-smart-contracts#resolver) on the Ethereum blockchain, which returns the `crypto.ETH.address` record attached to that domain. The resolved address is used to complete the ETH transfer to Ryan’s wallet.

![crypto payments success flow](../../images/crypto-payments-success-flow.png)

:::attention A domain can store many records and key formats
To learn about our supported record types, see our records reference guide.
:::

## Asking for help

Don't be shy... we're here to help. For assistance with integrating your app, please join our [Discord channel](https://discord.gg/b6ZVxSZ9Hn) for real-time support from UD and the community.