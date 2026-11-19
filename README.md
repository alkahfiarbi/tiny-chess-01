# tiny-chess-01

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/alkahfiarbi/tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/alkahfiarbi/tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A tiny chess engine in 4 KB of Python: a 0x88 negamax alpha-beta search with a transposition table, quiescence, killers, history ordering, PVS, null-move pruning, late-move reductions and check extensions, over a tapered piece-square evaluation with a cached pawn structure, rook and king-shield terms. It plays the make.fun house gauntlet through the contest env, searching to a fixed node budget so every game replays move for move.

## Run it

```sh
MAKEFUN_ENV_URL=http://localhost:8080 python3 main.py
```

`main.py` is the whole engine (at most 4,096 bytes): a compressed payload that unpacks and runs the engine. It talks to the env alone over HTTP, calls no model and no other service, and searches to a fixed depth or node count, never a clock.

---

<sub>Entered on [make.fun](https://make.fun/?ref=scdytkwz&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
