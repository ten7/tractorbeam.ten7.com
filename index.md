---
title: Home
layout: page
show_sidebar: false
hide_hero: true
---

# Tractorbeam


## Open source multi-tier website backups

Technology is fragile. When you think of sites going down, you usually think of big things like hacks, but entire systems of critical functionality could get lost if someone trips over a power plug. A thorough backup strategy is crucial to ensure that you can get your site back online quickly no matter what happens, whether the issue is site hacks, server problems, or zombie attacks.

We couldn’t find a backup solution that did everything we needed so we built our own: Tractorbeam, an open source, multi-tier, automated website backup tool that backs up your site code, database and site files.


*   **Tractorbeam does automated multi-tier backups daily, weekly and monthly, or any time schedule you choose.**
By default, Tractorbeam keeps seven daily backups, four weekly backups and twelve monthly backups. You could even configure the Docker container that runs Tractorbeam to run hourly backups. 
*   **Tractorbeam can write backups to any S3-compatible hosting provider, including Amazon AWS and Google Cloud.**
Tractorbeam can write backups to any S3 or Rsync destination you choose, 
*   **Tractorbeam keeps a set number of backups per timescale.**
The value of a backup decreases the older it gets. If you have a website problem you’re likely going to discover it pretty quickly, so the most recent backups are what you need. Unlike other rolling backup solutions, Tractorbeam automatically prunes old backups before it uploads them to S3 locations to save space. 
*   **Tractorbeam works on most types of hosting.**
    Tractorbeam needs to access databases (MySQL or MariaDB) and site files through SSH, which is available on most hosts. We also support [Pantheon](https://pantheon.io/) and [platform.sh](https://platform.sh/), because Tractorbeam can access files through the command-line tools from those providers.
*   **Tractorbeam is free and open source, so you have complete ownership of and access to your backups.**
    You only have to pay for the server Tractorbeam runs on, and the hosting of the backups themselves. For example, at Digital Ocean, you could pay $5/mo for [a droplet](https://www.digitalocean.com/products/droplets/?refcode=5fb69d9c62e4) and $5/mo for [Spaces](https://www.digitalocean.com/products/spaces/?refcode=5fb69d9c62e4) (their S3 storage) and be done. That's $10/mo for 250GB of storage and 1TB of bandwidth: more than enough for any number of websites.


## If your website host already has backups, why do you need Tractorbeam?

Because your host’s backups are likely in the same data center—if not the same server—that your site lives on. What if something happens to that server or that data center? Your site and your backups might be compromised. It always makes good business sense to have off-site backups in different geographical locations from your site host.

