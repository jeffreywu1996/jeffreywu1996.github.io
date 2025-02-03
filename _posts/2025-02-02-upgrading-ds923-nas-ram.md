---
layout: post
title: Upgrading My DS923+ NAS RAM - From 4GB to 32GB in My Homelab
category: Guides
---

I recently upgraded my Synology DS923+ from the factory 4GB to 32GB. In this post, I'll walk you through why I made the upgrade, how I chose the right memory modules, the installation process, and the performance gains I've seen so far.

## Why Upgrade?

- **Performance Boost & Caching:**
  Increasing the RAM in your NAS dramatically improves overall performance. More memory enhances caching, leading to snappier file transfers and smoother operation of applications like Docker.
- **Future-Proofing Your Homelab:**
  As my homelab grows—with more Docker containers and experimental projects—I need every ounce of performance available. Upgrading to 32GB now ensures that my system is ready for future demands.

## Choosing the Right Memory

Before purchasing, I conducted thorough research:
- **Community Feedback:**
  I scoured [the Synology RAM megathread on Reddit](https://www.reddit.com/r/synology/comments/16tmjoc/the_synology_ram_megathread_ii/) for success stories.
- **Aggregated Data:**
  I reviewed a [Google Sheet listing user experiences](https://docs.google.com/spreadsheets/d/13pJDfDot_7CmSWeo1jjbegM82QwQNIW0gFQ9o_4xhXA/edit?gid=1974572930#gid=1974572930) to narrow down my options.
- **My Selection:**
  I chose the memory available on [Amazon](https://www.amazon.com/dp/B0CCF65QG4?ref=ppx_yo2ov_dt_b_fed_asin_title) because it met all the necessary criteria (ECC, DDR4, compatible speed, and dual-rank configuration).

## Installation Walkthrough

### What You'll Need:
- **Synology DS923+ NAS** (with the original 4GB installed)
- **New RAM Modules:** Replacing the 4GB module with a new 32GB setup.
- **Anti-static Gloves & Proper Tools:** Essential to prevent static damage.

### Step-by-Step Process:
1. **Power Down & Disconnect:**
   Shut down your NAS (hold the power button for 3 seconds until you hear a beep) and unplug it from the mains. I even removed the hard drives—keeping note of their order—to ensure everything stayed secure.
2. **Remove Existing RAM:**
   Carefully eject the 4GB module using the side clips. Handle the memory by its edges.
3. **Install the New Modules:**
   Insert the new RAM sticks into the available SODIMM slots until they click into place.
   > **Tip:** Refer to this [YouTube tutorial on installing memory](https://www.youtube.com/watch?v=1Uj5uinv3nY) if you need extra guidance.
4. **Reassemble & Power Up:**
   Replace the drives, reconnect all cables, and power on your NAS. Once booted, verify that the new memory is recognized on the Synology DSM dashboard.

   ![Synology DSM showing 32GB RAM and cache usage](/assets/synology32gb.png)
   *Screenshot showing the upgraded 32GB RAM and cache usage*

## Running the Memory Test

After installation, verify that the new RAM is functioning correctly:
- **Using Synology Assistant:**
  Download the Synology Assistant from the [Synology Download Center](https://www.synology.com/en-us/support/download) and run the built-in memory test.
- **Memory Test Guidance:**
  I also followed this [YouTube guide on running the memory test](https://www.youtube.com/watch?v=3Ls5E5uTzVU) for additional insights.

## Observed Improvements & Future Plans

### Performance Gains:
- **Faster File Transfers:**
  The NAS now performs quicker indexing in Synology Drive and handles multitasking more fluidly.
- **Enhanced Docker Experience:**
  Enhanced reliability and responsiveness when running multiple Docker containers.

### What's Next?
- **Deep Dive into Docker:**
  Stay tuned for a follow-up post detailing Docker optimization techniques.
- **Monitoring & Benchmarking:**
  I plan to explore tools to track performance improvements over time.

## Lessons Learned and Tips

- **Double-Check Compatibility:**
  Ensure the memory stick is ECC, operates at the correct speed (DDR4 2666 or 3200MHz), and is a dual-rank module if required.
- **Handle with Care:**
  Use anti-static precautions during installation.
- **Leverage Community Insights:**
  Utilize forums and shared spreadsheets for guidance on NAS upgrades.

## Final Thoughts

Upgrading my DS923+ to 32GB has been a rewarding experience—improving performance and paving the way for future projects. I hope this guide helps you navigate your upgrade with confidence. Feel free to share your experiences or ask questions in the comments!

Happy upgrading!
