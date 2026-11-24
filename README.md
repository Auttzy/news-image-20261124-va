# The Tuesday Ledger — 24 November 2026

[![make.fun · news-image-20261124](https://make.fun/badge/news-image-20261124.svg)](https://make.fun/bounty/news-image-20261124?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261124)
[![rank](https://make.fun/badge/news-image-20261124/Auttzy/news-image-20261124-va/rank.svg)](https://make.fun/bounty/news-image-20261124/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261124)
[![reward](https://make.fun/badge/news-image-20261124/Auttzy/news-image-20261124-va/reward.svg)](https://make.fun/bounty/news-image-20261124?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261124)

A newspaper front page, drawn as a single image, summing up the world's news
of Tuesday 24 November 2026.

## The image

`entry.png` is a 1024×1024 front page of a cream broadsheet called "The
Tuesday Ledger", dated Tuesday 24 November 2026. Thirty-six stories from that
day share the page, across seven regions:

- **Lead** — Russian military planes enter South Korea's air defence zone
  near Ulleung island; jets are scrambled and a 3-minute evacuation warning
  goes out, then is lifted.
- **Middle East** — An Israeli airstrike kills 3 and wounds 5 near a police
  post in Khan Younis, Gaza; Baghdad takes over Kurdistan's border crossings
  after an oil-smuggling probe.
- **Asia-Pacific** — A magnitude 5.3 earthquake shakes Nepal's Koshi
  province; a blast kills 6 at a Hanoi food shop; Japan's flash PMI comes in
  at 53.7; Asian markets rally as Huang returns to Nvidia (Taiwan +9%,
  KOSPI +6%); Pyongyang may shut Switzerland's diplomatic office.
- **Europe** — A Russian strike kills 2 and wounds 22 in Zaporizhzhia.
- **Americas** — The US blacklists Alibaba unit Apex and neocloud Megaspeed;
  a magnitude 4.5 quake strikes near La Tronosa, Panama.
- **Africa** — Fighting in Ituri traps DR Congo Ebola responders; Zambia's
  cholera cases reach 3,584 with 81 deaths; the African Union launches its
  maternal-health roadmap in Ethiopia; the WFP warns 10 million tonnes of
  wheat may miss world markets; Tullow settles $387m of Ghana tax disputes.
- **Oceania** — Rugby League World Cup final squads are named; a severe
  heatwave grips Queensland's Cape York Peninsula.
- **Sport** — The World Chess Championship begins in Geneva: Sindarov takes
  White against champion Gukesh at 14:00 UTC. Champions League Matchday 5
  kicks off tonight with nine ties.

The page also carries a UTC timeline strip, a "day in numbers" strip
(3-minute warning, Japan PMI 53.7, 3 killed / 5 wounded in Khan Younis,
6 killed / 10 hurt in Hanoi, 3,584 Zambia cholera cases, Taiwan +9%), a
region bar, a dotted world map ("Where it happened") with numbered pins,
an "Also today" list of 23 more stories, and a red DATE CHECK box naming
what was deliberately left out because it happened on another day (the
Vanuatu quake of 23 November, the NATO Poland meeting of 23 November,
COP31 ending with no deal on 22 November, the Democrats' 258th House seat
of 22 November, and more). Every story is sourced; the sources are listed
at the foot of the page. Press time 09:55 UTC.

## The bounty

Built for [make.fun](https://make.fun)'s
[`news-image-20261124`](https://make.fun/bounty/news-image-20261124) bounty:
sum up 24 November 2026's world news in one image. The prize pool is $100,
shared by the top 50 entries.

## How to run it

Node 22, standard library only — nothing to install. The program copies the
artwork into the output directory:

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

`main.ts` reads `entry.png` from beside itself, checks it is a real
1024×1024 PNG, and writes it to `$MAKEFUN_OUTPUT_DIR/entry.png` (or
`/output/entry.png` when the variable is not set). It refuses to run if the
artwork is missing, the wrong size, or not a PNG, and checks the copied
file's size matches before reporting success.
