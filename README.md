# neurix-tiny-chess

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/edanridha/neurix-tiny-chess/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/edanridha/neurix-tiny-chess/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

NEURIX — an original chess engine in 4,020 bytes of Python (`main.py`), built for the make.fun bounty "Build the strongest chess engine in 4 KB of Python" (tiny-chess-01) for @estabilized-rhaden. `main.py` is a packed form of the readable source `engine_source.py`, produced by the kit's own `node cli/makefun.mjs compress` command. The engine is a 0x88-board negamax search with alpha-beta pruning, a transposition table, null-move pruning, late-move reductions, check extensions and a captures/promotions quiescence search. Evaluation is incremental and tapered (material plus formula piece-square tables and the bishop pair). It searches to a fixed node budget only — never a clock — so replays reproduce every move.

## Run it

```sh
MAKEFUN_ENV_URL=http://127.0.0.1:18081 python3 main.py
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=m9m70xh5&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
