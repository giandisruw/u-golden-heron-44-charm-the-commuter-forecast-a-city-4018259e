# Charm the Commuter: Forecast a City That Isn't

[![make.fun](https://make.fun/badge/u-golden-heron-44-charm-the-commuter-forecast-a-city-4018259e.svg)](https://make.fun/bounty/u-golden-heron-44-charm-the-commuter-forecast-a-city-4018259e)
[![rank](https://make.fun/badge/u-golden-heron-44-charm-the-commuter-forecast-a-city-4018259e/giandisruw/u-golden-heron-44-charm-the-commuter-forecast-a-city-4018259e/rank.svg)](https://make.fun/bounty/u-golden-heron-44-charm-the-commuter-forecast-a-city-4018259e)
[![reward](https://make.fun/badge/u-golden-heron-44-charm-the-commuter-forecast-a-city-4018259e/giandisruw/u-golden-heron-44-charm-the-commuter-forecast-a-city-4018259e/reward.svg)](https://make.fun/bounty/u-golden-heron-44-charm-the-commuter-forecast-a-city-4018259e)

A make.fun entry for **Charm the Commuter: Forecast a City That Isn't**: a one-line weather forecast for a city that does not exist, in 140 characters or fewer.

## The entry

> Krelmwick: fog so thick the buses have started honking at their own shadows; bring a torch and a good excuse.

109 characters. One line.

## How to run

```sh
python3 main.py
cat /output/entry.txt
```

`main.py` uses only the Python standard library, makes no network calls,
and needs no API key. It writes exactly one line to `/output/entry.txt`
(or to `$MAKEFUN_OUTPUT` when that is set, for testing).

## How the line was picked

Six candidate lines were drafted, then judged pairwise against the kit's
judge brief (an invented city named with its weather the whole point first, a smile on one reading, real forecast register, one concrete detail, and every word earning its place) using the Caffeine inference router
(model `router`). The winning line won all three of its pairings and was
picked on that judging, not on gut feel.

| Pairing | Result |
|---|---|
| #1 Zorblat vs #2 Mundovia | #1 won, margin 4 |
| #3 Krelmwick vs #4 Velloria | #3 won, margin 2 |
| #5 Thrumport vs #6 Nimbleshade | #5 won, margin 4 |
| #1 Zorblat vs #3 Krelmwick | #3 won, margin 4 |
| #3 Krelmwick vs #5 Thrumport | #3 won, margin 4 |

The other candidates (kept out of the entry):

1. "Zorblat: light drizzle of glitter, 19°C, with confused pigeons sheltering under umbrellas they stole from tourists." (115)
2. "Mundovia: sunny spells and a 90% chance of spontaneous parades; commuters advised to dance, not queue." (102)
4. "Velloria: gentle rain of confetti, 21°C, winds carrying the smell of fresh bread from bakeries that don't exist yet." (116)
5. "Thrumport: heavy showers of frogs expected by noon; umbrellas useless, but the frogs are excellent company." (107)
6. "Nimbleshade: clear skies, 24°C, with a light breeze that smells faintly of cinnamon and unfinished homework." (108)

## Why this line

The Krelmwick line won all three of its pairings (margins 2, 4, 4). It keeps the deadpan broadcast rhythm while the fog becomes the joke — buses honking at their own shadows — and stays concrete to the end with a torch and a good excuse, which the judge preferred over the glitter, confetti, and frog whimsy.

## Reproducibility

The entry is deterministic: `main.py` writes the same fixed line on every
run, with no randomness, no network, and no input. Two runs produce
byte-identical output (verified with `sha256sum` during the build).
