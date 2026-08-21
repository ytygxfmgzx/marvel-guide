# 豆瓣评分/链接填写清单

填写目标：每部电影在豆瓣的 **条目链接** 和 **评分**。
填好后，把内容贴回 `marvel_guide.html` 里的 `doubanData` 表（按 id 对应）。

## 怎么填

1. 打开 https://movie.douban.com ，搜每部电影的中文片名。
2. 点开正确的条目（注意核对年份），复制浏览器地址栏的网址。
3. 网页上「X.X」就是评分（取一位小数，如 `8.4`）。
4. 按下面的对应关系填入 `doubanData`。

## 填写格式（贴回 HTML 的 doubanData）

```js
const doubanData = {
    1:  { url: "https://movie.douban.com/subject/XXXXXXX/", rating: 8.4 },
    2:  { url: "https://movie.douban.com/subject/XXXXXXX/", rating: 6.8 },
    // ...没有的保留 url: "", rating: null
};
```

- `url`：豆瓣条目完整网址，用英文双引号包起来。
- `rating`：纯数字，不要加引号（写 `8.4`，不是 `"8.4"`）。
- 暂时没有的，保留 `url: "", rating: null` 即可，页面会自动显示「待填」或不显示徽章。

## 待填清单（28 部）

| id | 片名 | 英文/年份 | doubanData 键 |
|----|------|-----------|----------------|
| 1  | 钢铁侠 | Iron Man (2008) | `1: { url: "https://movie.douban.com/subject/1432146/", rating: 8.4 }` |
| 2  | 无敌浩克 | The Incredible Hulk (2008) | `2: { url: "https://movie.douban.com/subject/1866475/", rating: 7.1 }` |
| 3  | 钢铁侠2 | Iron Man 2 (2010) | `3: { url: "https://movie.douban.com/subject/3066739/", rating: 7.7 }` |
| 4  | 雷神 | Thor (2011) | `4: { url: "https://movie.douban.com/subject/1866471/", rating: 7.2 }` |
| 5  | 美国队长：复仇者先锋 | Captain America: The First Avenger (2011) | `5: { url: "https://movie.douban.com/subject/2138838/", rating: 7.2 }` |
| 6  | 复仇者联盟 | The Avengers (2012) | `6: { url: "https://movie.douban.com/subject/1866479/", rating: 8.3 }` |
| 7  | 钢铁侠3 | Iron Man 3 (2013) | `7: { url: "https://movie.douban.com/subject/3231742/", rating: 7.9 }` |
| 8  | 雷神2：黑暗世界 | Thor: The Dark World (2013) | `8: { url: "https://movie.douban.com/subject/6560058/", rating: 7.4 }` |
| 9  | 美国队长2：冬日战士 | Captain America: The Winter Soldier (2014) | `9: { url: "https://movie.douban.com/subject/6390823/", rating: 8.1 }` |
| 10 | 银河护卫队 | Guardians of the Galaxy (2014) | `10: { url: "https://movie.douban.com/subject/7065154/", rating: 8.1 }` |
| 11 | 复仇者联盟2：奥创纪元 | Avengers: Age of Ultron (2015) | `11: { url: "https://movie.douban.com/subject/10741834/", rating: 7.5 }` |
| 12 | 蚁人 | Ant-Man (2015) | `12: { url: "https://movie.douban.com/subject/1866473/", rating: 7.7 }` |
| 13 | 美国队长3：内战 | Captain America: Civil War (2016) | `13: { url: "https://movie.douban.com/subject/25820460/", rating: 7.9 }` |
| 14 | 奇异博士 | Doctor Strange (2016) | `14: { url: "https://movie.douban.com/subject/3025375/", rating: 7.6 }` |
| 15 | 银河护卫队2 | Guardians of the Galaxy Vol. 2 (2017) | `15: { url: "https://movie.douban.com/subject/25937854/", rating: 8.0 }` |
| 16 | 蜘蛛侠：英雄归来 | Spider-Man: Homecoming (2017) | `16: { url: "https://movie.douban.com/subject/24753477/", rating: 7.3 }` |
| 17 | 雷神3：诸神黄昏 | Thor: Ragnarok (2017) | `17: { url: "https://movie.douban.com/subject/25821634/", rating: 7.4 }` |
| 18 | 黑豹 | Black Panther (2018) | `18: { url: "https://movie.douban.com/subject/6390825/", rating: 6.5 }` |
| 19 | 复仇者联盟3：无限战争 | Avengers: Infinity War (2018) | `19: { url: "https://movie.douban.com/subject/24773958/", rating: 8.1 }` |
| 20 | 蚁人2：黄蜂女现身 | Ant-Man and the Wasp (2018) | `20: { url: "https://movie.douban.com/subject/26636712/", rating: 7.2 }` |
| 21 | 惊奇队长 | Captain Marvel (2019) | `21: { url: "https://movie.douban.com/subject/26213252/", rating: 6.8 }` |
| 22 | 复仇者联盟4：终局之战 | Avengers: Endgame (2019) | `22: { url: "https://movie.douban.com/subject/26100958/", rating: 8.5 }` |
| 23 | 蜘蛛侠：英雄远征 | Spider-Man: Far From Home (2019) | `23: { url: "https://movie.douban.com/subject/26931786/", rating: 7.6 }` |
| 24 | 黑寡妇 | Black Widow (2021) | `24: { url: "https://movie.douban.com/subject/25828589/", rating: 6.2 }` |
| 25 | 蜘蛛侠：英雄无归 | Spider-Man: No Way Home (2021) | `25: { url: "https://movie.douban.com/subject/26933210/", rating: 6.6 }` |
| 26 | 洛基 第一季 | Loki Season 1 (2021) | `26: { url: "https://movie.douban.com/subject/30331432/", rating: 8.5 }` |
| 27 | 奇异博士2：疯狂多元宇宙 | Doctor Strange in the Multiverse of Madness (2022) | `27: { url: "https://movie.douban.com/subject/30304994/", rating: 6.3 }` |
| 28 | 死侍与金刚狼 | Deadpool & Wolverine (2024) | `28: { url: "https://movie.douban.com/subject/26957900/", rating: 6.9 }` |

## 页面显示规则（自动，无需操心）

| 你填了什么 | 卡片徽章 | 详情弹窗 |
|------------|----------|----------|
| url + rating | `⭐ 8.4`（绿/橙/灰按分段），点击跳豆瓣 | 「⭐ 8.4」+「在豆瓣查看 ➔」 |
| 只填 url | 「豆瓣 ➔」黄色，点击跳转 | 「评分待填」+「在豆瓣查看 ➔」 |
| 只填 rating | `⭐ 8.4`，不可点击 | 「⭐ 8.4」+「链接待填」 |
| 都没填 | 不显示徽章 | 整个豆瓣区块隐藏 |

评分颜色分段：≥8 绿色，7~7.9 橙色，<7 灰色。
