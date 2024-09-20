# Game AB-Testing

Cookie Cats, a popular mobile puzzle game by Tactile Entertainment, challenges players to connect colored tiles to clear levels and features singing cats.

In this project, the impact of moving the first gate from level 30 to level 40 is analyzed through an A/B test, focusing on how this change affects player retention.

## Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Steps](#steps)
- [Conclusion](#conclusion)

## Overview

As players advance in the game, they encounter gates that either require a wait or an in-app purchase to continue. These gates not only drive purchases but also provide necessary breaks, potentially enhancing and extending player enjoyment.

The question is where to place these gates. Initially, the first gate was at level 30, but in this analysis, we examine an A/B test where it was moved to level 40. The focus is on assessing the impact on player retention. Before diving into the analysis, it's crucial to understand the data.

## Dataset

Data from 90,189 players who installed the game during the A/B test period includes the following variables:

- userid: A unique identifier for each player.
- version: Indicates whether the player was placed in the control group (gate_30, with a gate at level 30) or in the test group (gate_40, with the gate moved to level 40).
- sum_gamerounds: The total number of game rounds played by the player within the first 14 days after installation.
- retention_1: Indicates whether the player returned to play 1 day after installing the game.
- retention_7: Indicates whether the player returned to play 7 days after installing the game.

When a player installed the game, they were randomly assigned to either gate_30 or gate_40. As a preliminary check, let's ensure that both A/B groups have approximately the same number of players.

## Steps

I - Prepare Data

II - A/B Testing

III - Conclusion

## Conclusion

- The bootstrap analysis indicates strong evidence that 7-day retention is higher with the gate at level 30 compared to level 40. Thus, to maintain high retention rates, both 1-day and 7-day, it's better to keep the gate at level 30.

- While other metrics, like game rounds or in-game purchases, are also important, retention is crucial. Without retaining players, their spending becomes irrelevant

- One possible reason for higher retention at an earlier gate could be hedonic adaptation. This concept suggests that continuous engagement with a fun activity leads to reduced enjoyment over time. By placing the gate earlier, players take breaks and enjoy the game longer. If the gate is moved to level 40, fewer players reach it, and those who do may quit sooner due to boredom.

## Tools Used

- Pandas
- Matplotlib


