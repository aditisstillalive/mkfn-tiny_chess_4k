# mkfn-tiny_chess_4k

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/aditisstillalive/mkfn-tiny_chess_4k/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/aditisstillalive/mkfn-tiny_chess_4k/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A chess engine in under 4 KB of Python (`main.py`, an LZMA-packed source).
10x12 mailbox board that flips each ply, alpha-beta with PVS, transposition
table, null move, late-move reductions, check extensions, killers and a
quiescence search. Its eval is an incremental piece-square score whose
tables are rebuilt for each side at every root: game phase, passed and
isolated pawns, rooks on open files, king shelter and piece proximity to the
enemy king. Fixed node budget, no clock: the same position gets the same move.

## Run it

```sh
MAKEFUN_ENV_URL=http://localhost:8080 python3 -P -s main.py
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=hp5q8mh0&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
