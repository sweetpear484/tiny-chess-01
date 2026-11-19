# tiny-chess-01

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/sweetpear484/tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/sweetpear484/tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

An original chess engine in 4,091 bytes of Python (standard library only): 0x88 board, negamax alpha-beta with PVS, iterative deepening to a fixed 50,000-node budget per move (no clock anywhere, so every trial replays move-for-move), quiescence over captures, promotions and check evasions, a transposition table, MVV-LVA + killer + history move ordering, and a material + piece-square-table evaluation with bishop pair and endgame king centrality. In local practice trials on the kit's own scorer it rated Elo 1,451–1,545 against the house gauntlet.

## Run it

```sh
python3 main.py
```

The engine plays its games through the make.fun trial env: it reads `MAKEFUN_ENV_URL` (and `MAKEFUN_PROMPT_FILE` / `MAKEFUN_TRIAL_SEED`) from its environment and answers the env's `/game` and `/move` calls until every game is over.

---

<sub>Entered on [make.fun](https://make.fun/?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
