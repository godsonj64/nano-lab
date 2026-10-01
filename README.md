# nano-lab

Experiments with very small neural networks (architectures, training recipes and measurements), done in the open and pushed one day at a time.

This repository is rendered on the **Lab** page of my portfolio site. Every push updates it: the daily log, the experiment index, and a browsable, downloadable copy of every file.

## Layout

```
log/YYYY-MM-DD.md          one entry per day
experiments/<name>/        one folder per experiment (README.md + code + results)
templates/experiment/      copy this folder to start a new experiment
```

## Daily log

Add `log/YYYY-MM-DD.md`. Front matter is optional; without it the site uses the first heading and paragraph.

```md
---
title: Short title for the day
summary: One sentence for the timeline.
tags: [tokenizer, ablation]
---
```

## Experiments

Each `experiments/<name>/README.md` can declare:

| field     | meaning                                      |
|-----------|----------------------------------------------|
| `title`   | display name                                 |
| `summary` | one sentence: the question it answers        |
| `status`  | `planned`, `running`, `done` or `abandoned`  |
| `date`    | start date, `YYYY-MM-DD`                     |
| `tags`    | list of keywords                             |

Large artifacts (checkpoints, datasets) are git-ignored; publish them as release assets instead.

## License

MIT, see [LICENSE](LICENSE).
