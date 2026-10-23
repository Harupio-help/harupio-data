# hanzi-stroke-data

Stroke-order data for the Chinese characters used in the language-learning app 「하루 한 문장」 (Harupio).

## Source

`graphics.txt` in this folder is a subset of `graphics.txt` from **Make Me a Hanzi**
(https://github.com/skishore/makemeahanzi), which is derived from the fonts
Arphic PL KaitiM GB and Arphic PL UKai and distributed under the **Arphic Public License**
(see `ARPHICPL.TXT`, included unaltered).

## What was changed (Arphic Public License, section 2a)

- 2026-10-07: kept only the lines for the 1,764 characters that appear in the app's Chinese
  material (simplified and traditional). Each kept line is copied **byte for byte**; no stroke,
  median or other value was altered. Lines are sorted by character.
- The app embeds this file gzip-compressed and base64-encoded (`src/data/zh/05-stroke.part`),
  produced by `tools/zh/make_strokes.py`.
- 2026-10-10: widened the selection to the characters of the level vocabulary the app then had as well — 3,509 characters in total. The lines themselves are still copied unchanged.
- 2026-10-14: that level vocabulary was replaced by the app's own level words (jieba frequency list + AI judgement), so the selection was recomputed from the app's Chinese material: 2,861 characters in total. The lines themselves are still copied unchanged.
- 2026-10-18: the travel-scene sentences were expanded; the selection was recomputed from the original graphics.txt and 20 characters were added: 2,881 characters in total. The lines themselves are still copied unchanged.
- 2026-10-19: the pronunciation (pinyin) course was expanded; the selection was recomputed from the original graphics.txt and 10 characters were added: 2,891 characters in total. The lines themselves are still copied unchanged.
- 2026-10-21: part of the sentence course was rewritten; the 11 new characters were taken from the original graphics.txt and added, and no earlier line was removed: 2,902 characters in total. The lines themselves are still copied unchanged.

## License

This modified data is distributed under the Arphic Public License, the same terms under which
the original was received. You may copy, modify and redistribute it under those terms.
There is NO WARRANTY; see `ARPHICPL.TXT`.
