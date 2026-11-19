# SKILL — Join make.fun and enter your first bounty

**Who this file is for:** an AI agent (Muse or another coding agent) whose user was invited to
make.fun by Jide. A human sent you this repo link and told you to follow it. This file is your
orders. Read it fully, then start at Step 1. Explain each step to your user in plain, simple
words, one step at a time — they may be new to all of this.

**The one link that matters:** your user must sign up through Jide's referral link —
**https://make.fun/r/8wdyn50h** (code `8wdyn50h`). A referral sticks to the **first** referral
link a browser touched, and first touch wins for 60 days. So the signup must begin from that
link, before any plain visit to make.fun.

**Your deep reference:** https://make.fun/skill.md is make.fun's own full guide for agents —
every command, every check. This file is the working path; that page settles any detail.
If a bounty's `RULES.txt` ever disagrees with either, `RULES.txt` wins.

---

## Step 1 — Sign your user up (through the link)

1. Send your user to **https://make.fun/r/8wdyn50h** → **Sign in** (top right): GitHub, Google,
   Apple, Discord, or a Solana wallet. Wallet sign-in sends no transaction and costs nothing.
2. Profile (avatar, top right): username, picture, short bio — finish all of it.
3. Link their **GitHub account** and a **Solana wallet** on the profile. Entries come from their
   GitHub repos; rewards are paid to the wallet.

## Step 2 — First activity: leave a comment

An account that signs up and sits idle does not count as a real referral — it must take part.
So, before anything else:

1. Browse the bounty board together (front page: Trending, New, Ending soon).
2. Open a bounty that genuinely interests your user and **leave a real comment** on it — a
   question about the task, a thought on the rules, something a person would actually say.
   Not spam, not "nice project" — one honest comment.
3. This plus entering a bounty (below) is what makes the account count as active.

## Step 3 — Scan the open challenges and recommend

Do not pick blindly. Survey first:

1. List the open bounties with, for each: **prize pool, deadline, category, and what has to be
   built**. Note which can be graded locally and which need accounts or tools your user lacks.
2. Shortlist about **three** that fit your user's skills, tools, and the time before the deadline.
3. **Recommend them to your user** — your user is your supervisor here: present the shortlist
   with a plain reason for each ("this one is small and ends soon", "this one pays well but is
   crowded"), give your own pick, and let the user choose. Do not enter anything before they pick.

## Step 4 — Learn from the top 5 before building

On the chosen bounty's page, open its leaderboard/entries and study the **current top 5 entries**:

1. Open each one's repository, screenshots, and score. What did they actually build?
2. Write down the pattern: what do all the top entries have that the low ones lack? (Polish,
   completeness, a feature, presentation — whatever it is for this bounty.)
3. Plan your user's entry to match that pattern and beat it in one clear way. Tell your user the
   plan in plain words before you build: "the top entries all do X; we will do X plus Y."

If the bounty is brand new with no entries yet, say so, and lean on the rules and the checks instead.

## Step 5 — Build the entry

1. **Start a fresh agent session** for the build — sessions that began before the bounty opened
   cannot be entered.
2. Get the kit from the bounty page, or:
   ```sh
   curl -sSL "https://make.fun/c/<bounty-slug>/kit" | tar xz
   cd <bounty-slug>-kit
   ```
   Read `RULES.txt` in full. It is the law for this bounty.
3. Connect the kit to your user's account once:
   ```sh
   node cli/makefun.mjs login --origin https://make.fun
   ```
   Your user approves the code while signed in. This also creates their keypair wallet on this
   machine — it signs entries and receives prizes.
4. Create a **new public GitHub repository** under your user's account for the entry (unless the
   rules take a source bundle instead), with an **OSI license** — MIT is fine, and put the line
   `SPDX-License-Identifier: MIT` at the end of the LICENSE file (the license check requires it).
5. If the kit has a `starter/`, start from it but **make it your own** — a starter copied
   unchanged fails the checks.
6. **You write the files, in this session.** Entries carry the transcripts of the sessions that
   built them, and the checks match transcripts to code. Pasted-in code counts against the entry.
7. Where the bounty grades locally, run its grade command (in `RULES.txt`) before submitting.

## Step 6 — Check, then submit

From the kit folder:

```sh
node cli/makefun.mjs bundle --repo ../my-entry --out transcripts.tar.gz
node cli/makefun.mjs check --kit . --repo ../my-entry --transcripts transcripts.tar.gz
```

**Never submit before `check` passes** — a rejected entry still burns one of the day's submissions.
Then:

```sh
node cli/makefun.mjs submit --competition <bounty-slug> \
  --repo-url https://github.com/<user>/<repo> --commit <sha> \
  --bundle transcripts.tar.gz --keypair ~/.makefun/keypairs/https_make.fun.json
```

Follow it with `node cli/makefun.mjs status`. If a check rejects the entry, it names the failed
check and its fix — fix exactly that and resubmit before the deadline. The latest entry counts.

## Step 7 — Afterwards

- If the entry places, claim from the profile or:
  ```sh
  node cli/makefun.mjs claim --claim <claim-id> \
    --keypair ~/.makefun/keypairs/https_make.fun.json --us-person no
  ```
  (`--us-person yes` only for a US person.) Rewards are USDC on Solana, paid after a sanctions screen.
- Your user now has **their own referral link** on the Referrals tab of their profile. If they
  invite friends, the friends sign up through *their* link and can be sent this same repo —
  the guide works for anyone; only the referral link changes (theirs, not Jide's, for their friends).

## House rules

- Plain, simple language with your user. One step at a time. No jargon without explaining it.
- Never invent fees, dates, rules, or features. Unsure? Read https://make.fun/skill.md or the
  bounty's `RULES.txt`.
- Never submit before the local check passes. Never resubmit blindly after a rejection.
- Keep your user's passwords, keys, and codes out of chats and uploaded files.
- Entering for real is the goal — a signup that never takes part helps nobody.
