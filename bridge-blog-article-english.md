# What is sTokens Bridge? and How does it work?
Hi, I am Ikeda and have been developed in Dev protocol since September.
In this article, I will introduce a new contract, sTokens Bridge, which I have been developing recently.
The sTokens Bridge is not released yet (The source is here [github sTokensBridge](https://github.com/dev-protocol/s-tokens-bridge) ),
but in this article I will explain what this new contract will achieve in the future.

## Overview
The sTokens Bridge is a contract, where sTokens-holders deposit their STokens and get new ERC20 tokens in return.
The bridge gives a sTokens-holder as many ERC20 tokens as his staking amount
(To know what the sToken is, see this article: [sTokens, NFTs mirroring DEV staking](https://medium.com/devprtcl/stokens-nfts-mirroring-dev-staking-b41f93d0f8a6).
The sToken is an NFT which is the certificate of staking).

Creators of an OSS project can offer benefits to sTokens holders, 
and by doing so, the creators can gives stakers an incentive for long-term staking.
The new contract, sTokens Bridge, transform sTokens into ERC20 tokens.
By this transformation, 
the Bridge makes creator's benefit-offering more flexible and decentralized, thus it helps the OSS community to grow.

## Why is the sTokens Bridge necessary?
Here let us assume an situation where Alice stakes 98 DEVs in the Property "Ingram".
By this staking, Alice gets an NFT called sTokens
which has the following information: Property = Ingram, StakingAmount = 98 DEVs.
When Ingram creators want to offer benefits to Alice,
they have to check if Alice has a sToken whose property is Ingram,
and futhermore they need to know how many DEVs Alice is staking most of the time.

Now let us assume that the creators is trying to develop a Dapp, where Alice can take benefits form her sToken.
In such a Dapp, developers need to read the inner information of Alice's sTokens. 
However, to get the inner information,
they have to check the source code of the sTokens contract,
that is, they have to develop a Dapp to meet the unique specification of the sToken.

Isn't it a really bad idea that forcing developers to write codes to meet the sToken's unique specification.
That's why we introduce the sTokens Bridge. When Alice deposits her sTokens,
she get a certificate of staking and 98 Ingram ERC20 tokens which represents her staking amount.

What would it be if Alice could use this ingram token instead of the sToken itself?
In this case, the developers no longer need to read the inner information of the sToken.
Instead they only need to check the Alice's balance of Ingram tokens.
That is, the developer can use the ERC20 interface which is really standard and easy to develope with.
This clearly shows the sTokens Bridge improves the composability of the sToken.

## An example of application
An example of the Bridge application is the community governance.
Such a Dapp is already developed actually.
[Snapshot](snapshot.org) is a Dapp where users can vote by using ERC20 tokens as their voting right.
Like Snapshot we can use the Bridge tokens, that is, OSS creators can give each staker voting right which is proportional to one's Bridge token balance.
In this way the creators can make decisions about their project with respecting their supporter.

## Conclusion
sTokens can give opportunities where OSS creators offer benefits to stakers,
but it is inconvenient to check the staking amount of each staker.
The sTokens Bridge solve this inconvenience by transforming the sTokens into ERC20 tokens which is really standard and easy to develop with.
By introducing the sTokens Bridge, benefits-offering will be more active,
thus that would bring about the further growth of the DEV community.



