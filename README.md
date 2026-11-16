![Live rank](https://make.fun/badge/tiny-chess-01/achzul/tiny-chess/rank.svg)
![Live reward](https://make.fun/badge/tiny-chess-01/achzul/tiny-chess/reward.svg)

# tiny-chess

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/achzuldaf/tiny-chess/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/achzuldaf/tiny-chess/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A complete chess engine in one 4,083-byte `main.py` (Python 3.13, stdlib only): 0x88 board, negamax alpha-beta with principal-variation search and a transposition table, quiescence search, tapered piece-square tables, repetition detection. Fixed 60,000-node budget per move — never a clock — so games replay move for move. Packed by the kit's `makefun compress` from a readable 12,575-byte source. Perft-verified; Elo 1364 on the kit practice gauntlet (floor 1154).

## Run it

```sh
MAKEFUN_ENV_URL=http://127.0.0.1:8123 python3 main.py
```

Point `MAKEFUN_ENV_URL` at a tiny-chess-01 environment server from the competition kit; the engine loops on its `/game` and `/move` endpoints until the trial is done.

---

<sub>Entered on [make.fun](https://make.fun/?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
