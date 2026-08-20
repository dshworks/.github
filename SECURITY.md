# Security

Org-wide default for [dshworks](https://github.com/dshworks). A repo that
ships its own `SECURITY.md` overrides this one — `dsh-crew`, `dsh-meter`, and
`dsh-watch` each do, because a plugin that runs code on your machine owes you a
specific answer rather than a general one. Everything else in the org inherits
this page.

## What this org publishes

Two kinds of thing, with different risk shapes:

- **Plugins** you install into dsh, which execute in your session and read your
  workspace. Each carries its own `SECURITY.md` describing exactly what it
  touches, what needs a credential, and what runs without a model in the loop.
- **Registries and the sites that read them** — `awesome-dsh-plugins`,
  `awesome-dsh-themes`, `dsh.works`, `dshthemes.com`. These publish data *about*
  other people's code. They install nothing and they run nothing of yours.

## The registry risk nobody names

A directory's real vulnerability is not XSS on its own gallery. It is **listing
something harmful and lending it the credibility of having been listed.**

We try to make that failure small and legible rather than pretend it cannot
happen:

- An entry says what was actually checked and nothing more. `evidence` is a
  `path#key` you can click: this file, fetched from that repo's default branch,
  carries this key. That is a claim about an install path, **not a security
  review**, and the sites say so on the page.
- Nothing is promoted for money. The paid seats on both sites sit outside the
  data, in their own colour, marked as advertising, and cannot move a row.
- A git install runs code on your machine at install time, outside any sandbox.
  Being listed here changes nothing about that.

**If a listed repository is malicious, typosquatting, or has been taken over,
tell us and we will act on it before we finish arguing about the category.**
That is the report we most want to receive. A private advisory on the registry
repo is the fastest route; a plain issue is fine if the repo is already publicly
known to be bad, since there is no disclosure to protect at that point.

## Reporting

Open a private security advisory on the repo in question — `Security` >
`Report a vulnerability` — or a normal issue if the problem is not sensitive.
Expect a reply within a few days. These are small volunteer-maintained projects,
not products with an on-call rotation, and we would rather say that plainly than
publish a response-time promise we cannot keep.

Please do not put an API key, a session transcript, or a `.env` file in a
report. A redacted description of the behaviour is enough, and we would rather
not hold your secret while we read it.

## Out of scope

- Vulnerabilities in DeepSeek Harness itself. This org is not affiliated with
  DeepSeek; report those
  [upstream](https://github.com/deepseek-ai/deepseek-harness/security).
- Vulnerabilities in a third-party plugin we merely list. Report those to its
  author — and tell us too, so we can mark the row while it is unfixed.
