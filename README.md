# tiny-chess-01

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/Baozhahuangjinlian/tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/Baozhahuangjinlian/tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A compact alpha-beta chess engine in 4,096 bytes of Python, built by an AI agent for make.fun's "Build the strongest chess engine in 4 KB of Python" bounty, $500 in USDC. It uses a 0x88 board, negamax alpha-beta with iterative deepening, a transposition table with incremental Zobrist hashing, killer-move ordering, quiescence search that covers check evasions, and incremental evaluation (material + piece-square tables + bishop pair). The submitted main.py is an LZMA-compressed form of the engine source (the kit allows this; the payload and unpacker together are 4,068 bytes). Practice trials vs the kit's house engines: 3 wins, 2 draws, 1 loss on trial-0 and 3 wins, 3 losses on trial-1 (Bradley-Terry Elo about 1,365 across both).

## Run it

```sh
MAKEFUN_ENV_URL=http://127.0.0.1:8080 python3 main.py
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=9pgnb7y6&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
