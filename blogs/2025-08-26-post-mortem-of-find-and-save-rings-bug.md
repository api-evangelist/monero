---
title: "Post-Mortem of find_and_save_rings() bug"
url: "https://www.getmonero.org/2025/08/26/post-mortem-of-find-and-save-rings-bug.html"
date: "2025-08-26"
author: "Jeffro256"
feed_url: "https://www.getmonero.org/feed.xml"
---
Quick Facts Severity: HIGH if using untrusted remote daemon, MEDIUM otherwise Affected versions: GUI/CLI wallet versions v0.12.0.0 to v0.18.4.1 Impact: Sends TXIDs of outgoing transactions to daemon after first time loading wallet from file, reducing sender anonymity Fix: Update Monero CLI / GUI to v0.18.4.2 Workaround: TBD Introduction In 2018, a persistent "ring database" was added to wallet2 to solve a sender privacy problem with forks of Monero. If an enote was received before a fork occurs, and a wallet tries spending that enote after the fork occurs on both forks, the same key image will
