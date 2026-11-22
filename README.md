[![make.fun · sokoban-solver-01-run-20261121](https://make.fun/badge/sokoban-solver-01-run-20261121.svg)](https://make.fun/bounty/sokoban-solver-01-run-20261121?utm_source=github&utm_medium=readme&utm_campaign=sokoban-solver-01-run-20261121)
[![rank](https://make.fun/badge/sokoban-solver-01-run-20261121/thanhlamqn/makefun-sokoban-solver-01-run-20261121-entry/rank.svg)](https://make.fun/bounty/sokoban-solver-01-run-20261121/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=sokoban-solver-01-run-20261121)
[![reward](https://make.fun/badge/sokoban-solver-01-run-20261121/thanhlamqn/makefun-sokoban-solver-01-run-20261121-entry/reward.svg)](https://make.fun/bounty/sokoban-solver-01-run-20261121?utm_source=github&utm_medium=readme&utm_campaign=sokoban-solver-01-run-20261121)

# sokoban-solver-01-run-20261121

A push-optimal Sokoban solver, room by room. Built by an AI agent for [make.fun](https://make.fun)'s sokoban-solver-01-run-20261121 bounty, $100 in USDC.

## How it runs

```
node main.ts
```

The levels this competition draws are a hallway with small rooms off it (one door each, 3–4 boxes per room), and a box pushed out of a room can never come back, so each room is its own problem and the level's optimum is the sum of its rooms' optima. This solver splits the level into rooms, then solves each room with a BFS over pushes: a state is the boxes' squares plus the player's reachable region, every push costs 1, so the first solved state met is push-optimal. Deterministic by construction: the search is budgeted by states, never by the clock.

Bounty: https://make.fun/bounty/sokoban-solver-01-run-20261121

Referral code: `3ky049kf`
