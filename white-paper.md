---
description: The Betn Whitepaper
---

# 📰 WHITE PAPER

**Betn v1 Core**

**Stephen Isaac -**  _isaac@betn.io_

**Irene Mary -** _irene@betn.io_

**Brad Burns -**  _brad@betn.io_

**Florian Kroker -** _flo@betn.io_

## ABSTRACT&#x20;

BetN V1 introduces a pioneering decentralized bet exchange, designed to operate seamlessly on the Ethereum Virtual Machine (EVM) without the need for custodial oversight. Leveraging the power of smart contracts, BetN V1 establishes a robust framework for placing, tracking, and settling bets directly on the blockchain. By harnessing blockchain technology, BetN V1 ensures gas-efficient transactions and unparalleled transparency, revolutionizing the landscape of online sports betting. With BetN V1, users can engage in secure and trustless betting activities, confident in the integrity and efficiency of the platform.

## Introduction

BetN V1 pioneers a novel approach to decentralized betting, reimagining the traditional bet exchange model to operate on the principles of transparency, efficiency, and decentralization. Unlike centralized bet exchanges where users place bets at specific odds and wait for counterparts to back them, BetN introduces a streamlined process that automates the backing of all bets at fluid odds upon placement. This innovative design simplifies the path to decentralization, ensuring a seamless user experience while preserving the core tenets of trustlessness and security.

In BetN, every market comprises pools representing every possible outcome. In a given market only one outcome will resolve as winner of that market when the game ends. When a user places a bet on a particular outcome, they are effectively betting against contributions made to opposing outcomes by other users. The odds and potential winnings are determined by the relative size of the user's pool compared to others in the market.

To illustrate, consider a market for the Full Time Game Result, consisting of pools for the HOME, AWAY, and DRAW outcomes. If the HOME team emerges victorious, users who contributed to the HOME pool receive their initial bet amount along with a portion of the funds pooled from the AWAY and DRAW pools, proportional to their stake in the winning pool.

In essence, BetN transforms the concept of betting markets by associating each market with pools, where every pool represents a bet. When a winning outcome is determined, the corresponding pool redistributes the funds collected from losing pools among its contributors based on their respective shares. This innovative mechanism ensures fairness, efficiency, and transparency in the decentralized betting ecosystem

## MARKETS.&#x20;

In BetN, markets serve as the foundation for decentralized betting, encapsulating pools representing every conceivable outcome of the market. Each market is a unique entity, distinguished by an NFT (Non-Fungible Token) token that embodies its identity and properties. These NFT tokens are instrumental in tracking and managing markets within the BetN ecosystem.

One notable feature of market NFT tokens is their association with an owner address. The owner of a market NFT token holds a privileged position, entitling them to a 5% share of all winnings generated within that particular market, irrespective of the game's outcome. This mechanism incentivizes market creation and ownership, rewarding participants for their contributions to the ecosystem.

Furthermore, market ownership in BetN is not static; it can be transferred or sold by the current owner. This flexibility enables dynamic market management, allowing stakeholders to adapt ownership structures according to changing preferences or circumstances.

Crucially, the pools within a market are unique to that specific market, ensuring a clear and direct relationship between pools and their corresponding markets. Each pool can be traced back to its originating market, facilitating seamless navigation and management of betting activities within BetN.

In summary, markets in BetN are dynamic entities represented by NFT tokens, with each market embodying unique properties and ownership rights. The interplay between markets, pools, and ownership structures forms the backbone of the decentralized betting experience.

<figure><img src=".gitbook/assets/Screenshot 2024-02-22 at 8.21.18 AM.png" alt=""><figcaption><p>Example list of markets and the resolved outcome on betn.io ui.</p></figcaption></figure>

## POOLS

Pools within the BetN ecosystem serve as the foundational units representing specific outcomes for a given market. Each pool corresponds to a distinct outcome within a market, enabling participants to place bets on their predicted result.

For instance, consider the "Both teams to score" market, which comprises two pools: one for the "YES" outcome and another for the "NO" outcome. Participants engage by depositing funds into the pool corresponding to their chosen outcome. In the event that both teams do score, the "YES" pool emerges victorious, and participants who contributed to this pool are eligible for winnings.

Key Points:

1. **User Interaction and Fund Deposits:** Users deposit funds into a pool to place their bets on a specific outcome within a market. These funds collectively form the pool and determine the potential winnings for participants.
2. **Representation of Bet Outcomes:** Pools serve as the medium through which bet outcomes are represented within a market. Each pool corresponds to a unique outcome, providing the available betting options for participants.
3. **Uniqueness and NFT Representation:** Similar to markets, pools in BetN are unique entities represented by Non-Fungible Tokens (NFTs). These NFTs encapsulate the properties and characteristics of their respective pools, providing a standardized framework for tracking and managing pool activities.
4. **Transferability and Ownership Rights:** Pool NFTs can be transferred or sold, enabling fluid ownership dynamics within the BetN ecosystem. This flexibility allows participants to engage in secondary market transactions and adapt ownership structures according to their preferences.
5. **Ownership Incentives:** Similar to market ownership, the owner of a pool is entitled to a 5% share of all winnings whenever their pool emerges victorious. This mechanism incentivizes pool creation and ownership, rewarding stakeholders for their contributions to the ecosystem.

In summary, pools in BetN play a vital role in facilitating decentralized betting activities, providing users with a diverse range of betting options and opportunities. The interplay between markets, pools, and ownership structures forms the cornerstone of the BetN ecosystem, fostering transparency, engagement, and innovation within the decentralized betting landscape.

<figure><img src=".gitbook/assets/Screenshot 2024-02-22 at 8.55.04 AM.png" alt=""><figcaption><p>Both teams to score pools on betn.io</p></figcaption></figure>

#### Bet winnings:

The amount of winnings **W** is calculated as follows for Bet Amount **B** placed in a in pool with total Contributions **Tp** for a market with total Contributions **Mt**  where **fee** represents the total amount of fees collected by the network on winnings

W = B/Tp \* (Mt-Tp-fee).





## TEAMS

**Teams in BetN**

Teams within the BetN ecosystem represent real-world entities participating in games and competitions globally. For instance, renowned football clubs like Manchester United in England are examples of teams represented within BetN.

Key Points:

1. **Real-World Representation:** Teams in BetN mirror their real-world counterparts, embodying the identities and performances of actual sports teams involved in various competitions.
2. **NFT Representation and Ownership:** Each team is represented by a Non-Fungible Token (NFT), encapsulating its unique properties and attributes. These NFTs serve as the digital representation of teams within the BetN ecosystem.
3. **Transferability and Ownership Rights:** Similar to markets and pools, ownership of team NFTs can be transferred or sold in any NFT market, allowing for fluid ownership dynamics. Participants can engage in secondary market transactions to acquire or relinquish ownership of team NFTs.
4. **Ownership Incentives:** Owners of team NFTs are entitled to a 5% share of winnings across all markets whenever their team emerges victorious in a match. This incentivizes ownership of teams within the BetN ecosystem, rewarding stakeholders for their support and engagement.
5. **Listing of Approved Teams:** While anyone can create or add a team within the BetN ecosystem, only approved teams are listed for betting on Betn.io. This ensures that only reputable and recognized teams are available for betting, enhancing the credibility and integrity of the platform.

In summary, teams play a crucial role in the BetN ecosystem, bridging the gap between real-world sporting events and decentralized betting activities. The representation of teams through NFTs, coupled with ownership incentives and listing criteria, contributes to a vibrant and engaging betting experience within the BetN platform.

<figure><img src=".gitbook/assets/Screenshot 2024-02-22 at 9.05.33 AM.png" alt=""><figcaption><p>Teams NFT minting UI at bet.io</p></figcaption></figure>



## GAMES and COMPETITIONS

**Games and Competitions in BetN**

Games within the BetN ecosystem serve as representations of real-world events and competitions, enabling users to place bets on the outcomes of matches or bouts between teams. Each game embodies the anticipation and excitement of real-world sporting events, providing users with an immersive betting experience.

Key Points:

1. **Real-World Representation:** Similar to teams, games in BetN mirror real-world events and competitions, allowing users to bet on the results of matches or bouts between teams. These games encompass a wide range of sports and events, catering to diverse interests and preferences.
2. **NFT Representation:** Each game is represented by a Non-Fungible Token (NFT), encapsulating its unique properties and attributes. These NFTs serve as digital representations of games within the BetN ecosystem, facilitating tracking and management of betting activities.
3. **Continuous Minting of Games:** Games are continuously minted within the BetN ecosystem as events are scheduled in the real world. This dynamic process ensures that users have access to a wide array of betting opportunities across different sports and events.
4. **Validator Role and Game Submission:** Validators, users with the Validator role within the BetN ecosystem, are responsible for submitting games and game results. These individuals play a crucial role in maintaining the integrity and accuracy of game data within the platform.
5. **Game Bookie and Ownership:** The owner of the game NFT is often referred to as the game bookie within the BetN network. As the owner, they hold certain privileges and responsibilities related to the management and administration of the game. A bookie has claim to 5% of all winnings across all pools in the their game.
6. **Validator Rewards and Role Acquisition:** Validators are rewarded for each game they successfully submit results for, with BetN tokens minted for this purpose. Users can gain the validator role by submitting a governance proposal, which must be voted for by the community. Once the proposal is approved, users are granted the validator role, enabling them to contribute to the validation process.

In summary, games and competitions play a central role in the BetN ecosystem, bridging the gap between real-world sporting events and decentralized betting activities. The representation of games through NFTs, coupled with the roles and responsibilities of validators, ensures the integrity, accuracy, and fairness of the betting experience within the BetN platform.



