---
title: "Deprecating Monero's Custom Transaction Unlock Time"
url: "https://www.getmonero.org/2026/05/10/deprecating-unlock-time.html"
date: "2026-05-10"
author: "Justin Berman (j-berman)"
feed_url: "https://www.getmonero.org/feed.xml"
---
Please be advised, the Custom Transaction Unlock Time feature is set to be deprecated at consensus with FCMP++. There is already a relay rule in place today that prevents nodes from accepting and relaying transactions with a Custom Unlock Time to the transaction pool ( source ). This is a formal announcement that the feature would be deprecated altogether with the FCMP++ fork, and new transactions with Custom Unlock Time set would not be able to enter the chain even if a miner mines them.
