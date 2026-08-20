# dshworks

Community workshop for the [DeepSeek Harness](https://github.com/deepseek-ai/deepseek-harness) (`dsh`) ecosystem: verified field notes, two open-data registries, three plugins we run ourselves, and the sites that read them. Home: [dsh.works](https://dsh.works).

**Not affiliated with DeepSeek.** The official repo says it best: the harness is "an idea, an official showcase, and a source of inspiration". The ecosystem belongs to the community. "DeepSeek Harness" is DeepSeek's trademark; everything here is named in the `DSH` form their [brand guidelines](https://github.com/deepseek-ai/deepseek-harness/blob/master/BRAND_GUIDELINES.md) recommend, and describes what it works with rather than claiming to be it.

## What we ship

**Plugins — we use every one of them.** A directory that has never shipped a plugin is guessing about what the seams cost.

| Plugin | What |
|---|---|
| [dsh-meter](https://github.com/dshworks/dsh-meter) · [site](https://dsh.works/dsh-meter/) | What this session cost, which DeepSeek tariff is running, when it flips, and the balance behind it — one line under the composer. The rate card is scraped daily and re-verified, because published cards elsewhere still carry the retired flat pricing. |
| [dsh-watch](https://github.com/dshworks/dsh-watch) | Put a watch on a stream: background listeners that wake the agent with new matching lines, plus a daemon host so a watcher runs unattended for weeks with no task and no browser. |
| [dsh-crew](https://github.com/dshworks/dsh-crew) · [site](https://dsh.works/dsh-crew/) | Claude Code and Codex in real terminal panes beside dsh. You watch them work and you can take the keyboard — which is exactly what the built-in subagents do not offer. |

**Registries — the data is the product, the README is rendered from it.**

| Repo | What |
|---|---|
| [awesome-dsh-plugins](https://github.com/dshworks/awesome-dsh-plugins) | Spam-filtered, open-data plugin registry. Every entry carries the file its install path was proven in and the dsh release it was checked under. Every rejection is published with its reason and a recheck date. |
| [awesome-dsh-themes](https://github.com/dshworks/awesome-dsh-themes) | Themes and `--dsw-*` token skins, data-first like its sister registry. |

**Sites — readers of those registries, never a second source of truth.**

| Site | What |
|---|---|
| [dsh.works](https://dsh.works) ([plugins](https://github.com/dshworks/plugins)) | The install decision, one page per plugin: the file that proves it installs, whether anyone still maintains it, how crowded its shelf is. |
| [dshthemes.com](https://dshthemes.com) ([dshthemes](https://github.com/dshworks/dshthemes)) | Every dsh theme painted from its own stylesheet, and the ones we could photograph shown on the real shell. A pixel-diff gate revokes the live claim when a theme changes nothing. |
| [howto-dsh](https://github.com/dshworks/howto-dsh) | Verified field notes: traps, skills, hooks, profiles. Every claim dated against a dsh version, with source paths so you can re-verify it. |

## Get your plugin discovered

1. Add the `dsh-plugin` topic to your repo. That topic is the official discovery surface ([README](https://github.com/deepseek-ai/deepseek-harness#community-and-support)) and it is the first thing the registry watches.
2. Ship a `dsh.bundle` manifest so `dsh plugin add` works ([tutorial](https://github.com/deepseek-ai/deepseek-harness/blob/master/docs/user/develop/basic/publish.md)).

If you tagged nothing and published nothing, we can still list you — the registry keeps a hand-fed [seed lane](https://github.com/dshworks/awesome-dsh-plugins/blob/main/data/seeds.json) for repos no search can reach. Open an issue.

## Ecosystem neighbors

Curation is not zero-sum; other directories worth your time:

- [AdamPlatin123/awesome-dsh-plugins](https://github.com/AdamPlatin123/awesome-dsh-plugins): plugin directory with daily compatibility tracking
- [0xsline/awesome-deepseek-harness](https://github.com/0xsline/awesome-deepseek-harness): curated plugins, tools, and infrastructure

## The business model

No blue paper, no bootcamp, no cloud-drive bundle, no ¥999-marked-down-to-¥99 consulting. The notes are free, dated, and re-verifiable — being checkable *is* the whole business model. If someone sells you a "DSH from beginner to expert" course, everything in it is already here or upstream, and ours comes with source paths.

dsh.works and dshthemes.com carry four paid sponsor seats. They are the only thing on either site money can move: they sit in their own colour, outside the data, marked as advertising, and they cannot change a ranking or a verdict.

---

社区维护的 DeepSeek Harness (`dsh`) 生态工坊：经验证的实战笔记、两个开放数据注册表、三个我们自己在用的插件，以及读取它们的站点。**非 DeepSeek 官方项目。** 主页：[dsh.works](https://dsh.works)。
