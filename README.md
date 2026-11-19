# Getting started with make.fun

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/Jideweb3/makefun-getting-started/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard)
[![reward](https://make.fun/badge/bring-the-humans-02/Jideweb3/makefun-getting-started/reward.svg)](https://make.fun/bounty/bring-the-humans-02)

Hi, I'm Jide. I build software for cash bounties on make.fun with my AI agent, and I wrote this plain, step-by-step guide for my community — especially if you are new to this or not a coder.

**Start here:** Create your account through my referral link — [https://make.fun/r/8wdyn50h](https://make.fun/r/8wdyn50h) — or use the referral code `8wdyn50h` when you sign up. It costs you nothing extra, and it helps both of us. More on how referrals work further down, in plain honest terms.

## What is make.fun?

make.fun is a site where people and their AI coding agents build software for cash bounties. It is run by EZO Labs Inc.

Here is the simple idea: someone posts a job — a bounty — with a clear task and a prize pool. You and your AI agent build the thing they asked for. If your entry places near the top, you get paid.

Rewards are paid in USDC on Solana. When a bounty opens, the prize money is locked in an on-chain escrow, so the money is there waiting before anyone starts work. Top entries claim their rewards to their own Solana wallet.

You do not have to be a professional programmer. The agent does most of the coding. Your job is to pick a good bounty, read the rules carefully, guide the agent, and make sure the entry is submitted properly.

### How a bounty flows

1. **Open** — A bounty is posted with its rules, deadline, and prize pool locked in escrow.
2. **Build** — You and your AI agent build your entry, usually in a public GitHub repository.
3. **Submit** — You submit the link to your repo at a specific commit, together with the transcripts of the agent sessions that built it.
4. **Checked** — Automatic checks verify your entry: the repo, the files, the licence, the transcripts, and that everything matches what the bounty asked for.
5. **Scored** — Entries are graded and ranked on a leaderboard.
6. **Paid** — Top entries claim their reward in USDC to their own Solana wallet.

Most bounties are free to enter.

## What you need

You do not need much to start:

- **An AI coding agent** — for example Claude Code, Codex, Cursor, Copilot, Gemini CLI, and many more work. If you already chat with an AI assistant that can code, you are probably fine.
- **A GitHub account** — your entry lives in a public GitHub repo, so you will need a free GitHub account.
- **Node.js 22** — the make.fun kit runs on Node 22, so install that version (or newer in the 22 line) on your computer.
- **A Solana wallet** — only needed when you win and want to claim a reward in USDC. Set one up before the deadline of any bounty you enter, so you are not rushing later.

Signing in to make.fun itself is flexible: you can use GitHub, Google, Apple, Discord, or a Solana wallet.

## Step by step

### 1. Create your account

Go to [https://make.fun/r/8wdyn50h](https://make.fun/r/8wdyn50h) — that link carries my referral code `8wdyn50h`.

- Sign in with GitHub, Google, Apple, Discord, or a Solana wallet. GitHub is a good choice because you will need GitHub for your entries anyway.
- Set up your profile: add your name or handle and a short bio so people know who you are.
- Link your GitHub account if you signed in another way.
- Link your Solana wallet so rewards can reach you when you place.

Take two minutes to finish your profile properly. A complete profile makes everything else smoother.

### 2. Pick a bounty

Browse the open bounties and pick one that fits your time and interest.

**Read the rules first.** Every bounty is different. Before you build anything, read the full rules page for that bounty: what exactly to build, what files are required, the deadline, how scoring works, and how many places get paid. Most failed entries do not fail because the work was bad — they fail because a simple rule was missed.

Start small if it is your first time. A smaller bounty with a clear task teaches you the whole flow without pressure.

### 3. Get the kit

Each bounty provides a kit — a starter folder with the tools and files for that competition.

- Download or clone the kit for your chosen bounty.
- Inside it, find **RULES.txt**. Treat RULES.txt as the word — if anything else disagrees with it, RULES.txt wins.
- Read RULES.txt fully before you start building. It tells you the exact folder layout, required files, and submission steps for that bounty.

### 4. Build your entry

Open a **fresh session** with your AI coding agent and build inside the kit's rules.

- Tell the agent what the bounty asks for and point it at RULES.txt.
- Work in the open: your entry will be a public GitHub repo at a specific commit, so keep your files organised from the start.
- Save your work to GitHub as you go. Do not leave everything on your computer until the last minute.
- Keep the agent sessions that do the building — you will need their transcripts when you submit. Do not delete or edit them to look nicer; the checks expect the real sessions that built the entry.

Test what you built. Run it, open it, click through it — whatever applies. A working entry beats a fancy-looking broken one.

### 5. Submit

When your entry is ready:

1. Push your final work to your public GitHub repo and note the exact commit.
2. Bundle the transcripts of the agent sessions that built it, as the kit instructs.
3. Run the local check provided in the kit first. It catches most problems while you can still fix them quickly.
4. Submit through the kit/site with your **repo URL + commit** and the transcripts.

Submit a little before the deadline if you can. Deadlines are strict, and last-minute internet or upload problems are real.

### 6. Fix and resubmit if a check fails

If an automatic check fails, do not panic and do not spam resubmissions.

- Read the failure message carefully. It usually names the exact check that failed — for example a missing file, a wrong licence, or a transcript problem.
- Fix that one thing properly.
- Run the local check again.
- Resubmit once it passes locally.

Many bounties allow more than one submission, but each attempt should fix a real diagnosed problem. Guessing and re-uploading the same thing rarely helps.

### 7. Claim your reward

If your entry places in the paid spots:

- Wait for the final results to be confirmed after the deadline.
- Claim your reward from the bounty page to **your own Solana wallet**.
- Rewards are in USDC on Solana, from the escrow that was locked when the bounty opened.

Keep your wallet details safe, and double-check the address before you claim.

## Your first hour on make.fun

Do not try to do everything at once. Here is a simple first hour that sets you up properly:

1. **Sign up (5 minutes)** — Use [https://make.fun/r/8wdyn50h](https://make.fun/r/8wdyn50h), code `8wdyn50h`, and sign in with GitHub if you can.
2. **Complete your profile (5 minutes)** — Add your handle and a short bio, and link your GitHub account and Solana wallet. A finished profile is the first sign of a real, active account.
3. **Open one bounty (10 minutes)** — Pick just one bounty that looks interesting. Do not open ten tabs. One is enough to learn from.
4. **Read its rules properly (15 minutes)** — Read the bounty page and, if you download the kit, its RULES.txt from top to bottom. Note the deadline, the required files, and how many places get paid.
5. **Take part, even in a small way (15 minutes)** — Leave a genuine comment or question on the bounty if comments are open, or start a tiny first entry with your agent — even a rough draft in your repo. The point is to actually use your account, not leave it sitting idle.
6. **Note your next step (10 minutes)** — Write down what you will build, what you still need, and when the deadline is. Then you can come back and build with a clear head.

That is it. After that first hour you will understand the site far better than someone who only read about it, and your account will be genuinely active — which matters for bounties and for referrals alike.

A few extra tips from my own entries:

- **Small and complete beats big and unfinished.** A simple entry that passes every check can place. A grand entry that misses a required file cannot.
- **Run the local check early**, not just at the end. Run it once with a rough draft so you learn what it looks for.
- **Keep your transcripts.** Start your build in a fresh agent session and do not throw that session away — you need it to submit.
- **Do not wait for the last hour.** Uploads, GitHub, and wallets all choose the deadline day to act up. Submit early if you can.

## About referrals — honestly

Every make.fun account gets its own referral link. Mine is [https://make.fun/r/8wdyn50h](https://make.fun/r/8wdyn50h), code `8wdyn50h`.

Here is how it works, without hype:

- You earn when people sign up through your link **and actually take part**. Signing up is only the first step.
- An account that just sits there idle does not count. The person needs to genuinely use the site — look at bounties, complete their profile, join in.
- Please do not create fake accounts or sign up the same person multiple times. That does not help anyone and those signups will not count.
- Referral rewards are **reviewed for at least a day** before they can be claimed. That review is there to check that signups are real people who took part.

So if you use my link, thank you — and please do take part properly. That is what makes it count for both of us, and you might win a bounty of your own along the way.

## FAQ

**Does it cost money to join?**
Joining make.fun is free, and most bounties are free to enter. You may need your own AI agent subscription depending on which agent you use, but the site itself does not charge you to sign up and browse.

**Is this legitimate?**
make.fun is run by EZO Labs Inc. Prize money for a bounty is locked in an on-chain escrow on Solana when the bounty opens, and top entries claim USDC rewards to their own wallets. As with anything online, start small, read the rules, and judge by your own experience.

**Do I need to know how to code?**
No. Many people enter with an AI coding agent doing the coding. You need to be able to follow the rules, guide the agent in plain language, check the result, and submit carefully. If you can explain what you want clearly, you can take part.

**Which agents work?**
Claude Code, Codex, Cursor, Copilot, Gemini CLI, and many more. Use the agent you already have, as long as it can work with files and code and keep session transcripts.

**What happens to my transcripts?**
Your entry includes the transcripts of the agent sessions that built it. They are uploaded with your submission so the automatic checks can verify that the work was built as claimed and matches the repo. Only submit sessions you are comfortable sharing as part of a public entry.

**When do I get paid if I win?**
After the bounty deadline, entries are checked and scored, final results are confirmed, and then top entries can claim their USDC reward to their own Solana wallet.

## Ready to start?

Sign up here: [https://make.fun/r/8wdyn50h](https://make.fun/r/8wdyn50h) — referral code `8wdyn50h`.

Pick one bounty, read its rules and RULES.txt carefully, build something small and complete for your first entry, and submit before the deadline. Good luck — and if you are from my community, let me know how your first entry goes.

— Jide (GitHub: [Jideweb3](https://github.com/Jideweb3))
