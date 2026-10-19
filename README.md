# 3-30-300 v2 (trial)

A trial version of the [3-30-300 map of Zuid-Holland](https://robertotjesse.github.io/3-30-300-regel/).
Map: https://robertotjesse.github.io/3-30-300-v2/

What is new compared with the main map:

- A first tab, 3·30·300, that combines the 3, the 30 and the 300 in one map. Sliders set
  how much each part counts. Every home gets a score per part (rule met yes/no, or a
  gradual score from 0 to the target), and a gemeente, wijk or buurt gets the mean of its
  homes. The popups also show the share of homes that meet all three, without weights.
- Two optional layers on every tab, for the groups most sensitive to heat: residents aged
  65 and older per 100 m square, and births per buurt (CBS 2024). CBS has no age group
  for 0 to 4 years, and births per 100 m square are nearly all suppressed, so births per
  buurt are the nearest count of babies.

This is a trial. The paper behind the rule gives no weights: each of the three is a
minimum. An average lets a good score on one part make up for a poor one on another,
so a buurt can look fine on this tab while hardly any home meets all three. Read the
combined tab together with the share that meets all three.

The site is static files only: `index.html`, the explanation pages in `uitleg/` and the
vector tiles in `data/`. The code that builds the tiles is on the branch
[`test/samen-gewogen`](https://github.com/RobertoTjesse/3-30-300-regel/tree/test/samen-gewogen)
of the main repository (`web/build_tiles_samen.py`, `web/build_tiles_kwetsbaar.py`).
