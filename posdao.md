---
description: >-
  Bet Results are submitted via a proof of stake voting system referred to as
  Betn Posdao. Validators are responsible for submitting results and they form
  the backbone of  the betn network.
---

# ⏱️ POSDAO

**BetN Validators: Guardians of Decentralized Betting**

In the intricate ecosystem of BetN, validators stand as the guardians of decentralized betting, ensuring the accuracy and integrity of game results through a proof of stake voting system known as BetN Posdao. Validators play a pivotal role in upholding the reliability and trustworthiness of the BetN network, forming its backbone and driving its evolution.

Key Points:

1. **Responsibilities of Validators:** Validators are entrusted with the critical task of submitting game results on the BetN network. They validate game outcomes, verify their accuracy, and ensure that only true results are accepted within the ecosystem.
2. **Scale and Deployment:** The BetN network is designed to support up to 5000 validators, underscoring the scale and robustness of the platform. Initially, the BetN team creates the first five validators to kickstart the network, while ten additional slots are available on a first-come, first-serve basis for users seeking to purchase the validator role.
3. **Community Governance and Role Acquisition:** As governance transitions to the community, more members will have the opportunity to become validators through a democratic process. Users can request to become validators via a governance proposal, with approval granting them the role on the contract. Similarly, users can request the removal of validators through the same proposal process.
4. **Qualifications and Commitment:** Validators are expected to be passionate about sports and committed to serving the betting community. Individuals with expertise in sports data analysis or access to reliable results sources are well-suited for the role. Validators must demonstrate a deep understanding of sports dynamics and exhibit a strong drive to uphold the integrity of the BetN platform.
5. **Staking Requirement and Rewards:** Validators must stake 10,000 BETN tokens to claim the role, representing a significant financial commitment. This staked amount is refunded by 50% once the validator renounces or is stripped of the role. Validators are compensated for their work through the BETN token, with rewards distributed based on their contributions to the network.
6. **Results Consensus and Token Rewards:** Validators stake an amount of BETN tokens when submitting results, with the maximum reward amount currently being minted associated with the submission. If a validator's result aligns with a previous submission, a vote is conducted to back that result. Once 51% of validators support a submission, it is deemed the true result. Validators who stake on incorrect results forfeit their stake, which is redistributed among backers of the true result.

In summary, validators in BetN play a pivotal role in maintaining the integrity and reliability of decentralized betting. Their commitment to accuracy, expertise in sports, and dedication to community service are essential pillars of the BetN ecosystem, driving its success and sustainability.

#### At launch  (Before Governance kicks in) , this is what is required to become a validator



1. **10000 BETN token burn**.  Since at the initial stage there is not enough BETN in circulation, a special contract has been created  to mint **10000** BETN tokens to interested Validators. The initial purchase from this contract will be valued at 30BNB for 10500BETN.&#x20;
2. Once the  Purchased 10000 BETN tokens have been burned at the POSDAO. the user will automatically receive the validator role. Please NOTE, before governance the BETN team will have the full authority revoke any validator  roles.
3. In order to provide results and Claim the Validator reward, the validator will have to stake another 50-100 BETN on each results set provided.
4. Once the number of validators  reaches 50. the result reward will be slashed to 30 BETN. if this occurs before governance, the team will effect it. if after, it will be brought to a vote via proposal.



### **REWARDS.**



Rewards are distributed in diminishing amounts via; **first come - first serve.**

As of the time of writing, The full reward Amount is currently 300 BETN for min of 12 validators.

The max reward per validator is currently set at 50 BETN. This is also the stake amount required to submit results.

Lets see how the algorithm distributes the rewards for the first 15 Submissions. based on position

```php

1 => 50.00 // reserved for 10 minutes for the bookie.
2 => 41.67 // second person to submit
3 => 34.72
4 => 28.94
5 => 24.11
6 => 20.09
7 => 16.74
8 => 13.95
9 => 11.63
10 => 9.69
11 => 8.08
12 => 6.73
13 => 5.61
14 => 4.67
15 => 3.89
```

Total 16 validators will receive above 3 BETN token

total amount => 294.57 BETN for validators receiving over 1 BETN.

The minimum winning Vote for this spread is also set to 12, since other validators earning under 1 BETN may not have the incentive to vote. this does not mean they cannot vote!!

Once a pool reached 12 votes, the results will be finalized

**#1 Top position earning 50 BETN is reserved for the game Bookie for up to 10 Minutes**. After Ten minutes, if the game bookie has not claimed the reward, any validator can take this position.

The Algorithm can be adjusted to support more or less validators by reducing or increasing  the the max reward  or total reward per result.



Lets see an example with the Max reward/Stake per validator now raised to 200 BETN for a total of 2000 BETN distribution.



<pre class="language-php"><code class="lang-php"><strong>  0 => 200.0
</strong>  1 => 180.0
  2 => 162.0
  3 => 145.8
  4 => 131.22
  5 => 118.098
  6 => 106.2882
  7 => 95.65938
  8 => 86.093442
  9 => 77.4840978
  10 => 69.73568802
  11 => 62.762119218
  12 => 56.4859072962
  13 => 50.83731656658
  14 => 45.753584909922
  15 => 41.17822641893
  16 => 37.060403777037
  17 => 33.354363399333
  18 => 30.0189270594
  19 => 27.01703435346
  20 => 24.315330918114
  21 => 21.883797826302
  22 => 19.695418043672
  23 => 17.725876239305
  24 => 15.953288615375
  25 => 14.357959753837
  26 => 12.922163778453
  27 => 11.629947400608
  28 => 10.466952660547
  29 => 9.4202573944925
  30 => 8.4782316550432
  31 => 7.6304084895389
  32 => 6.867367640585
  33 => 6.1806308765265
  34 => 5.5625677888739
  35 => 5.0063110099865
  36 => 4.5056799089878
  37 => 4.0551119180891
  38 => 3.6496007262802
  39 => 3.2846406536521
  40 => 2.9561765882869
  41 => 2.6605589294582
  42 => 2.3945030365124
  43 => 2.1550527328612
  44 => 1.939547459575
  45 => 1.7455927136175
  46 => 1.5710334422558
  47 => 1.4139300980302
  48 => 1.2725370882272
  49 => 1.1452833794045
  50 => 1.030755041464 
</code></pre>

TOTAL 1990.7 BETN.

As you can see, we now have over 51 validators Earning over 1 BETN. Validators claiming under 1 BETN can still vote but the incentive will be low. they could just vote to swing the results

The Min votes in this case will now be 25 votes.

These setting will all be adjustable via the governance protocol.

This system is designed to push validators to quickly submit results as the longer they take, the lesser the reward they could earn. The system also allows for less staking when more validators join the network.\


## BOOKIES

**Bookies in BetN: The Showrunners of Decentralized Betting**

In the innovative landscape of BetN, bookies assume a pivotal role as the showrunners of decentralized betting. Unlike traditional bet exchanges, where bookies back bets, BetN bookies facilitate games by orchestrating various stages of the betting process.

Key Points:

1. **Game Facilitation:** Facilitating games involves several key responsibilities, including adding the game to the contract, promoting the game to users, and ultimately committing the results of the game. Bookies are the driving force behind these activities, ensuring the smooth execution of each stage.
2. **Showrunner Role:** Bookies act as the showrunners of the game, overseeing its entire lifecycle from inception to resolution. They play a central role in ensuring the integrity, fairness, and transparency of the betting process within the BetN platform.
3. **Earning Potential:** Bookies enjoy a unique earning opportunity, as they are entitled to 5% of all winnings generated from games facilitated by them. This incentivizes active participation and responsible management of games within the platform.
4. **Validator Delegation:** To become a bookie, a user must first hold the validator role, which is acquired through delegation by other members. Validators who lose their validator status also forfeit their privileges as bookies, ensuring that only trusted and active participants serve in this capacity.
5. **Reward Structure:** Bookies earn rewards through the BetN PoSDao contract, similar to other validators. However, bookies enjoy a special ten-minute window to claim the first spot in the result submission line, maximizing their potential rewards, since he first submitter earns the highest amount of rewards.

In summary, bookies in BetN serve as the linchpins of decentralized betting, orchestrating games and ensuring the integrity of the platform. Their dual role as validators and facilitators positions them at the forefront of the betting experience, driving engagement and fostering trust within the BetN community.















