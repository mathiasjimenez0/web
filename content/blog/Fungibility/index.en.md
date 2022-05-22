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

The primary two standards for token creation in Ethereum smart contracts are ERC-20 and ERC-271, used for fungible and non-fungible token creation respectively. Standardizations are useful because they allow composability, meaning that in a smart contract one can easily call functions defined in other smart contracts. For example, this allows for one token created in a smart contract to be traded in a decentralized exchange created by other smart contracts. I argue here that economically speaking, the extent of fungibility embedded in any economic good is ultimately subjective, which implies that more objective aspects of the technological design of the good in question do not determine its fungibility, although they can certainly affect people's subjective assessments.

Fungibility is the extent to which economic agents *perceive* different physical realities as interchangeable (which includes digital goods since these are just graphical renders of information bits). But since this characterization resides on agents' perception of realities, no economic good is intrinsically more fungible than another. Even more, no physical reality is intrinsically an economic good. Instead, the fungibility of a class of physical realities depends on whether the agent perceives these realities as potentially providing different services, or in other words, if the sources of utility from holding or consuming different units of this class of goods vary across units. Even more, the sole aggregation of physical realities to define a "class" done by any third party is ultimately somewhat arbitrary.

Let me now give some examples of this principle. First, think about what people usually think as the most fungible goods, monies. Why are these fungible? While coinage and printing technologies, or the equivalent spendability of all monetary units in any deposit contract play a role, in the end what matters is people's perceptions about these characteristics. For example, coins and bills offered could be considered as counterfeited or too worn, which depends on sellers' subjective assessments. As for bank deposits, without deposit insurance, the same monetary unit at different banks can be priced differently by different people, for instance due to different perceptions about the risk of default across people and banks. 

As for more non-fungible economic goods, think first about a simple example of two persons buying socks. While the first one only cares about their softness, the second also cares about their colors. Therefore, only for the latter person socks are going to be non-fungible. Are the different Bored Apes NFTs objectively non-fungible? In principle, nothing impedes each of these tokens from being perceived as interchangeable. One could even try an experiment with NFTs to prove the point of this post. Deploy a smart contract with ERC-271 standards such that all collection units are exactly the same, but at some future point, all of these become of a different color. Make two of these collections, run two auctions with different sets of potential buyers, and tell about this change of color to only one of them. Suppose the market prices for units are different only for the collection with knowledgeable buyers. In that case, this might suggest that units become non-fungible only because buyers perceive them like this and not because we used an ERC-271 standard for creating them.
