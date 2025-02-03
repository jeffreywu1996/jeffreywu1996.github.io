---
layout: post
title: Upgrading My DS923+ NAS RAM - From 4GB to 32GB in My Homelab
category: Guides
---

I recently upgraded my Synology DS923+ from the factory 4GB to a whopping 32GB. In this post, I'll walk you through why I made the upgrade, how I chose the right memory modules, the installation process, and the performance gains I've seen so far.

## Why Upgrade?

- **Performance Boost & Caching:**
  Many online experts and forum discussions agree that increasing the RAM in your NAS can dramatically improve overall performance. More memory isn't just for multitasking; it's also used for caching frequently accessed data, leading to snappier file transfers and smoother operation of applications like Docker.
- **Future-Proofing Your Homelab:**
  As my homelab grows—with more Docker containers and various experimental projects—I need every ounce of performance I can get. Upgrading to 32GB now means I won't be scrambling for a new upgrade when workloads increase.

## Choosing the Right Memory

Before purchasing, I did my homework:
- **Community Research:**
  I scoured [the Synology RAM megathread on Reddit](https://www.reddit.com/r/synology/comments/16tmjoc/the_synology_ram_megathread_ii/) to see which memory modules other users have had success with.
- **Aggregated User Feedback:**
  I also checked out a [Google Sheet listing reported experiences with different RAM sticks](https://docs.google.com/spreadsheets/d/13pJDfDot_7CmSWeo1jjbegM82QwQNIW0gFQ9o_4xhXA/edit?gid=1974572930#gid=1974572930) that helped narrow down the options.
- **My Pick:**
  Ultimately, I chose the memory stick available on [Amazon](https://www.amazon.com/dp/B0CCF65QG4?ref=ppx_yo2ov_dt_b_fed_asin_title) because it met all the criteria (ECC, DDR4, compatible speed, and dual-rank configuration) recommended by fellow NAS enthusiasts.

## Installation Walkthrough

### What You'll Need:
- **Synology DS923+ NAS** (with the original 4GB installed)
- **New RAM Modules:** My upgrade consisted of replacing the old module with a new 32GB setup.
- **Anti-static Gloves & Proper Tools:** To avoid any static damage. (Not really)

### Step-by-Step Process:
1. **Power Down & Disconnect:**
   Completely shut down (hold power button for 3 seconds until you hear beep) your NAS and unplug it from the mains. I even removed the hard drives (and noted their order) to ensure nothing was accidentally knocked out during the upgrade.

2. **Remove Existing RAM:**
   Carefully eject the 4GB module using the side clips. Handle the memory by its edges to avoid touching the chips.

3. **Install the New Modules:**
   Firmly insert the new RAM sticks into the available SODIMM slots, ensuring they click into place.
   > **Tip:** Follow a [YouTube tutorial on how to install the memory](https://www.youtube.com/watch?v=1Uj5uinv3nY) if you're unsure about the process.

4. **Reassemble & Power Up:**
   Replace your drives, reconnect all cables, and power on your NAS. After booting, check the Synology DSM dashboard to see the new memory recognized.

   ![Synology DSM showing 32GB RAM and cache usage](https://user-images.githubusercontent.com/13981821/synology32gb.png)
   *Screenshot showing the upgraded 32GB RAM and how much is being used for system cache*

## Running the Memory Test

After installation, it's crucial to verify that the new RAM is functioning correctly:
- **Using Synology Assistant:**
  Download and install the Synology Assistant from the [Synology Download Center](https://www.synology.com/en-us/support/download) (if you haven't already). Then, run the built-in memory test to ensure no errors occur.
- **Memory Test Video Tutorial:**
  I followed another helpful [YouTube guide on running the memory test](https://www.youtube.com/watch?v=3Ls5E5uTzVU) that showed how to interpret DSM's memory info.

## Observed Improvements & Future Plans

### Performance Gains:
- **Faster File Transfers:**
  The NAS is noticeably snappier, with quicker indexing in Synology Drive and smoother multitasking.
- **Enhanced Docker Experience:**
  Running multiple Docker containers has become more reliable and responsive, which is key as I experiment with various applications.

### What's Next?
- **Deep Dive Into Docker:**
  Stay tuned for a follow-up post where I'll detail the Docker apps I'm hosting and share tips on optimizing container performance on Synology.
- **Monitoring & Benchmarking:**
  I plan to explore tools and methods for tracking performance improvements over time, comparing resource usage before and after the upgrade.

## Lessons Learned and Tips for Fellow Enthusiasts

- **Double-Check Compatibility:**
  Always verify that the memory stick is ECC and the correct speed (DDR4 2666 or 3200MHz, as recommended) and check that it's a dual-rank module if your NAS requires it.
- **Handle With Care:**
  Use anti-static precautions during installation to avoid damaging sensitive components.
- **Community is Gold:**
  Leverage forums and shared spreadsheets to learn from the collective experiences of other NAS users.

## Final Thoughts

Upgrading my DS923+ to 32GB has been a rewarding experience—one that not only improved performance but also set the stage for future projects in my homelab. I hope this guide helps you navigate your own upgrade with confidence. Feel free to drop a comment below with your questions or share your own upgrade stories!

Happy upgrading!
