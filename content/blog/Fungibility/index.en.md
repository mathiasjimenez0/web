---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Token Fungibility and Subjectivity"
subtitle: ""
summary: ""
authors: []
tags: []
categories: []
date: 2021-12-02T00:17:08-08:00
lastmod: 2021-12-02T00:17:08-08:00
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
---

ERC denominations within the Ethereum DeFi ecosystem refer to different standards for creating tokens with smart contracts. These contracts automatically control the issuance, distribution, transfer, and burning of tokens with several standard functions. These standardizations are relevant because they allow composability of contracts and protocols, meaning that one knows how to call a function in a smart contract from another smart contract. For example, this allows for one token created within a protocol to be traded in a decentralized exchange created for another protocol.

The primary two standards for token creation within Ethereum are ERC-20 and ERC-271, used to create fungible and non-fungible tokens, respectively. Here, however, I argue that economically speaking, the extent of fungibility embedded in any economic good is ultimately subjective, although this characterization can be affected by the technological design of the good in question.

Fungibility is the extent to which economic agents *perceive* different physical realities as interchangeable (which includes digital goods since these are just graphical renders of information bits). But since this characterization resides on agents' perception of realities, no economic good is intrinsically more fungible than another. Even more, no physical reality is intrinsically an economic good. Instead, the fungibility of a class of physical realities depends on whether the agent perceives these realities as potentially providing different service abilities. This is if the sources or levels of utility from holding or consuming different units of this class of goods vary. Moreover, any aggregation of physical realities to define a "class" done by any third party is ultimately somewhat arbitrary.

Let me now give several examples of this principle. First, think about probably the most fungible goods, monies. Why are monies fungible? Surely this is related to their technological properties, such as uniform coinage and paper bill printing, or the equivalent spendability of all units of bank deposits. However, this per-se doesn't determine the fungibility of monies. For example, before the advancement of coinage technologies, these were not always indistinguishable from the human eye's perspective. Therefore, a seller had to choose whether to accept the coin "by tale", or to make a discount on its value. Regarding banknotes, aside from the fact that some people might not accept wore or broken bills, there is also the issue of banknote liquidity. When redeeming privately issued banknotes depended on having a branch close by, a seller could make a discount depending on his disutility from transporting this bill to the nearest redeeming place, which could be thousands of kilometers away.

As for more non-fungible economic goods, think first about a simple example of two persons buying socks. While the first one only cares about their softness, the second also cares about their colors. Therefore, only for the latter person socks are going to be non-fungible. Are the different Bored Apes NFTs non-fungible? In principle, nothing impedes each of these tokens from being perceived as interchangeable. One could even try an experiment with NFTs to prove the point of this post. Deploy a smart contract with ERC-271 standards such that all collection units are exactly the same, but at some future point, all of these become of a different color. Make two of these collections, run two auctions with different sets of potential buyers, and tell about this change of color to only one of them. Suppose the market prices for units are different only for the collection with knowledgeable buyers. In that case, this might suggest that units become non-fungible only because buyers perceive them like this and not because we used an ERC-271 standard for creating them.
