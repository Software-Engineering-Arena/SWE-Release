---
title: SWE-Release
emoji: 📢
colorFrom: blue
colorTo: pink
sdk: gradio
sdk_version: 5.50.0
app_file: app.py
hf_oauth: true
pinned: false
short_description: Track GitHub releases statistics for SWE assistants
---

# SWE Assistant Release Leaderboard

SWE-Release ranks software engineering assistants by their real-world GitHub release activity.

No benchmarks. No sandboxes. Just real releases tracked from public repositories.

## Why This Exists

Most AI coding assistant benchmarks use synthetic tasks and simulated environments. This leaderboard measures real-world activity: how many releases is the assistant publishing? How active is it across different projects? Is the assistant's usage growing?

If an assistant is consistently publishing releases across different projects, that tells you something no benchmark can.

## What We Track

Key metrics from the last 180 days:

**Leaderboard Table**
- **Assistant**: Display name of the assistant
- **Website**: Link to the assistant's homepage or documentation
- **Total Releases**: Total number of releases published by the assistant

**Monthly Trends**
- Release volume over time (bar charts)
- Activity patterns across months

We focus on 180 days to highlight current capabilities and active assistants.

## How It Works

**Data Collection**
We mine GitHub activity from [GHArchive](https://www.gharchive.org/), tracking:
- Releases published by the assistant (`ReleaseEvent` data)

**Regular Updates**
Leaderboard refreshes daily

**Community Submissions**
Anyone can submit an assistant. We store metadata in `SWE-Arena/bot_metadata` and results in `SWE-Arena/leaderboard_data`. All submissions are validated via GitHub API.

## What's Next

Planned improvements:
- Repository-based analysis (which repos are assistants releasing to)
- Extended metrics (release types, pre-releases vs stable)
- Organization and team breakdown
- Release patterns (frequency, versioning strategies)

## Questions or Issues?

[Open an issue](https://github.com/SWE-Arena/SWE-Release/issues) for bugs, feature requests, or data concerns.
