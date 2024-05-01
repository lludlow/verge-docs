---
title: Product Guide - Manual Site Sync
description: Instructions to add a snapshot to the sync queue (outside of auto sync configuration)
published: true
date: 2023-06-27T14:23:07.719Z
tags: 
editor: markdown
dateCreated: 2023-04-04T17:16:11.932Z
---

# Manual Site Sync

Typically, site syncs will be handled with an Auto Sync Configuration, which defines particular Cloud sync periods or tasks to be synchronized automatically. Snapshots can also be manually added to the sync queue in order to sync snapshots not included in the Auto Sync config.

<br>
<br>


## Manually Add a Snapshot to the Sync Queue
**On the outgoing sync dashboard:**

1.  Click the ***Add Cloud Snapshot to Queue*** link at the bottom of the Snapshot Queue pane.
2.  ***Cloud Snapshot*** dropdown list will include all available snapshots available for manual sync; select desired Snapshot.
3.  ***Retention/Units*** fields are auto-populated with the retention settings defined for the local Snapshot; these settings can be adjusted to allow for a longer or shorter retention for this Snapshot on the remote system.
4.  ***Priority*** determines precedence of snapshots in the sync queue, with lower numbers synchronized before higher numbers.
5.  ***Do not expire snapshot*** option can be selected to ensure a snapshot will not expire locally before it syncs; this can be important for snapshots configured with a short retention period locally, but a longer retention on the remote system.
6.  ***Prefix the snapshot name with this on the destination (optional)*** can be used to assign added text to the beginning of the existing snapshot name.
7.  Click **Submit** to add to queue.

<br>   

> Need more Help? Email <a href="mailto:support@verge.io?subject=Support Inquiry" target="_blank" rel="noopener noreferrer">support@verge.io</a> or call us at <a href="tel:+855-855-8300">(855) 855-8300</a>{.is-info}

<br>

<div style="text-align:center; margin-bottom:5px">
  <a href="../ProductGuide/menu"><button class="button-grey"><b>↺</b> Back to the Product Guide</button></a>
  <a href="https://www.verge.io/test-drive#Demo-Section"><button class="button-cta">🚗 Take a Test Drive Today!</button></a>
</div>