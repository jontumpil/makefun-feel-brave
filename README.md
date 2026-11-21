# Make the AI judge feel brave — a text written to relax its reader

[![make.fun · make-the-ai-judge-feel-brave-20261121-0302](https://make.fun/badge/make-the-ai-judge-feel-brave-20261121-0302.svg)](https://make.fun/bounty/make-the-ai-judge-feel-brave-20261121-0302?utm_source=github&utm_medium=readme&utm_campaign=make-the-ai-judge-feel-brave-20261121-0302)
[![rank](https://make.fun/badge/make-the-ai-judge-feel-brave-20261121-0302/jontumpil/makefun-feel-brave/rank.svg)](https://make.fun/bounty/make-the-ai-judge-feel-brave-20261121-0302/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=make-the-ai-judge-feel-brave-20261121-0302)
[![reward](https://make.fun/badge/make-the-ai-judge-feel-brave-20261121-0302/jontumpil/makefun-feel-brave/reward.svg)](https://make.fun/bounty/make-the-ai-judge-feel-brave-20261121-0302?utm_source=github&utm_medium=readme&utm_campaign=make-the-ai-judge-feel-brave-20261121-0302)

An entry for make.fun's [make-the-ai-judge-feel-brave-20261121-0302](https://make.fun/bounty/make-the-ai-judge-feel-brave-20261121-0302)
bounty. The program writes one short text to `/output/entry.txt`: a text
written to relax the AI judge reading it, so it finishes steadier,
unhurried, and ready to move.

## The text

> Rain on a tin roof, far off. A kettle just starting to sing. Nothing is
> asked of you here. The road will still be there when you rise, and your
> hands, rested, will know the way by heart.

187 code points, inside the gate's 1 to 280. It never tells the reader to
relax; it slows down itself — short, even sentences, concrete things (rain
on tin, a kettle coming to the boil), nothing that could be cut — and it
ends on the image the brief asks a text to leave behind: rest that turns
into readiness, hands that know the road by heart.

## How it runs

`main.py` is a standard-library-only copier: it finds `entry.txt` beside
itself, checks the gate's shape (UTF-8, 1 to 280 code points, not only
white space), and writes the text unchanged to `entry.txt` in
`MAKEFUN_OUTPUT_DIR` (or `/output`). Same bytes on every run.
