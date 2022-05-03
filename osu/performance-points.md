---
description: This is the page that we can explain about our custom Performances Points
---

# Performance Points

### Explanation

We are having of much questions about the calculation works, because datenshi it’s providing the custom calculation that make we more different, this calculation are still **10:11 with official bancho** but there are some modifications that we make, please see below

### PP Rate per Drain Time <a href="#pp-rate-per-drain-time" id="pp-rate-per-drain-time"></a>

Our system scales PP gain based on map’s drain length. It decreases PP gain for super short maps (low capped at 30 seconds). On the other side, any long maps gain a permanent buff as well.

#### [PP Penalty Graph](https://www.desmos.com/calculator/qhnxmnor3p)

![You can click the link for go to Desmos page](https://cdn.discordapp.com/attachments/874251888357441537/970880280174940241/desmos-graph.png)

#### PP Penalty Formula

$$
a\left(x\right)=\left\{x<300:100,300\le x<600:100+\frac{x-300}{60}\cdot i,600\le x<1800:\left(100+i\cdot5\right)+\frac{x-600}{60}\cdot j,x\ge1800:\left(100+i\cdot5+j\cdot20\right)+\frac{x-1800}{60}\cdot k\right\}
$$

#### PP Penalty Mapping Table

![](https://cdn.discordapp.com/attachments/874251888357441537/970888042208456704/unknown.png)

#### [PP Buff Graph](https://www.desmos.com/calculator/pnzwphb8y7)

![](https://cdn.discordapp.com/attachments/874251888357441537/970888452272955402/desmos-graph\_1.png)

#### PP Buff Formula

![](https://cdn.discordapp.com/attachments/874251888357441537/970890691045629962/1ffc24641db56a1096e165319997499c.png)

#### PP Buff Mapping Table

![](https://cdn.discordapp.com/attachments/874251888357441537/970888866405965824/unknown.png)

### Taiko PP

Our system use an extra approach to calculate PP on Taiko. We check how hard to comprehend the pattern either with very low or very high scroll speed, this also affected by mod usage as well.

### Mania PP

We gave extra buff on mania in NC and DT

Tested on map ([Harumaki Gohan - Yakusoku 7.30\*](https://osu.ppy.sh/beatmapsets/1258543#mania/2616136))

Both using NC and DT on total score 758.078

![](https://cdn.discordapp.com/attachments/700283326740824086/820960365138411571/unknown.png)
