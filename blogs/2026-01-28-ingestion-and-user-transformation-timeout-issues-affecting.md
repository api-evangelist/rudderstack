---
title: "Ingestion and user transformation timeout issues affecting a subset of the EU customers"
url: "https://status.rudderstack.com/incidents/tm6b00ntcpcc"
date: "2026-01-28"
feed_url: "https://status.rudderstack.com/history.atom"
---
Jan 28 , 22:49 UTC Resolved - Between 21:55 - 22:25 UTC RudderStack experienced a temporary ingestion issue which caused 5xx errors on ingestion for a subset of the EU customers. Based on the retry logic of the SDK, these events were likely retried but there might have been some data loss for Server Side SDK's during this timeframe. Also between 21:09 - 22:00 UTC we have observed timeout errors on some of the user transformation code executions that would have dropped the events.
