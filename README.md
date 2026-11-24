# tiny-chess

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/mrblack193/tiny-chess/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/mrblack193/tiny-chess/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A tiny original chess engine in 4 KB of Python: alpha-beta search with quiescence, transposition table, killer moves and piece-square evaluation. Written from scratch for the make.fun bounty.

## Strength

Local practice trials against the house gauntlet (kit env + scorer): Elo 1,191 / 1,099 / 1,279, mean ~1,190 — above the 1,154 floor to enter the final. Fixed 50,000-node search, about 1.2 s per move, deterministic (no clock, no randomness).

## Run it

```sh
python3 main.py
```

It plays through the trial env at `MAKEFUN_ENV_URL` (`POST /game`, `POST /move`) and exits when every game is over. No model calls, no other network, no files read besides the env.

---

<sub>Entered on [make.fun](https://make.fun/?ref=80g65mgt&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
