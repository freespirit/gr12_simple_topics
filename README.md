# About

A simple analysis of the top topics in GR12.

(in `gr12_eda.ipynb`)

# How
Based on keyword extraction we can see what topics were most interesting and most supported by individual contributors.

The total crowdloan amount is used as criteria which grants are most supported.

## Keyword extraction
It's a relatively simple NLP task but for simplicity of the setup we use the handy OpenAI API - we can simply call the
API with a text and receive the keywords. No need to setup our own environment, especially with a GPU and maintain models, etc.

# Results
The results can be seen at the end of the notebook as Conclusions but you can scroll up to
see more detailed keywords. Or just here:

**GR12**
> ZigZag Exchange - ZigZag, DEX, StarkNet, zkSync, Starkware.

> Dark Forest - blockchain games, decentralized games, zkSNARKs, Ethereum.

> Coin Center is educating policy makers about public blockchains - Bitcoin, cryptocurrency, blockchain, policy research.

**GR11**
> Dark Forest - zkSNARKs, blockchain gaming, Ethereum, xDAI.

> ETHPlanet - member of togETHer - ethereum, blockchain, smart contract, dapp, solidity.

> Nym - Nym, privacy, anonymity, unlinkability, decentralized mixnet, blockchain.

## Conclusion
Can we say something about the topics of the most crowdfunded grants? We can conclude that:
* blockchain games (GameFi, etc.) remain a hot topic. Particularly - Dark Forest is among top 3 in two consecutive rounds
* rollups, L2, etc. became more popular
* privacy and anonymity gave way to policy and research
* the top 3 GR12 grants have attracted 2.5x more crowdfunded amounts - from ~160k to ~425k
* the number of unique contributors (total for top 3) has almost doubled - from ~14k to ~27k

# Gotchas
Texts of grants are not programmatically available so they were copied manually from each grant's
webpage (top 3 only). Watch out for long texts!

GPT3 is not deterministic and sometimes it returns an empty set of keywords or slightly different
ones. To fix that one needs to tweak its parameters but that's not the topic of the task. A few runs prove 
that the results are mostly similar and are good enough to paint the picture.
