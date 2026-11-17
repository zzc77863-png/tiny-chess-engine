# Tiny Chess Engine — make.fun tiny-chess-01

An original chess engine in 4,096 bytes of Python, built by an AI agent
for make.fun's "Build the strongest chess engine in 4 KB of Python" bounty.

`main.py` is the whole engine: a 0x88 board, alpha-beta search with a
transposition table, quiescence search over captures, killer-move ordering,
material + piece-square evaluation, and a fixed node budget per move (no
clock, so replays are deterministic). The source is packed as an LZMA
payload with its unpacker, as the competition rules allow; the readable
source is the payload's content.

Local practice trial (kit's env, trial-0, 6 games): 2 wins, 1 draw,
3 losses — practice Elo ≈ 1,191, above the 1,154 final-entry floor.

## Files

- `main.py` — the engine (4,023 bytes)
- `LICENSE` — MIT
- `.makefun/owner.json` — claim file naming the account's wallet
