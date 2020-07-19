---
title: Home
layout: page
show_sidebar: false
hide_hero: true
---

# Tractorbeam


<img src="/images/logo.svg" class="is-pulled-right is-one-third" width="33%"/>

## Open source multi-tier website backups

Tractorbeam is a Docker container that can back up your entire website from a variety of hosts to S3-compatible object stores like AWS S3, [DigitalOcean Spaces](https://www.digitalocean.com/products/spaces/?refcode=5fb69d9c62e4), Google Cloud Storage, Ceph Object Storage, and more.  All libraries and utilities are built in to the container, so there's nothing more you need.


## If your website's host already has backups, why do you need Tractorbeam?

Because your host’s backups are likely in the same place as your site. What if something happens to that data center? Your site and your backups might be compromised. It always makes good business sense to have off-site backups. [Tractorbeam can help you get there!](/support/)


## Using Tractorbeam

Run the single shot container on your own infrastructure, see [tractorbeam.me/setup](/setup/) for details.


## What it does

*   **Tractorbeam does multi-tier backups daily, weekly and monthly.**
By default, Tractorbeam keeps seven daily backups, four weekly backups and twelve monthly backups. You could even configure the Docker container that runs Tractorbeam to run hourly backups. 
*   **Tractorbeam can write backups to any S3-compatible hosting provider, including Amazon AWS and Google Cloud.**
Tractorbeam can write backups to any S3 or Rsync destination you choose, 
*   **Tractorbeam keeps a set number of backups per timescale.**
The value of a backup decreases the older it gets. If you have a website problem you’re likely going to discover it pretty quickly, so the most recent backups are what you need. Unlike other rolling backup solutions, Tractorbeam automatically prunes old backups before it uploads them to S3 locations to save space. 
*   **Tractorbeam works on most types of hosting.**
    Tractorbeam needs to access databases (MySQL or MariaDB) and site files through SSH, which is available on most hosts. We also support [Pantheon](https://pantheon.io/) and [platform.sh](https://platform.sh/), because Tractorbeam can access files through the command-line tools from those providers.
*   **Tractorbeam is free and open source, so you have complete ownership of and access to your backups.**
    You only have to pay for the server Tractorbeam runs on, and the hosting of the backups themselves. For example, at Digital Ocean, you could pay $5/mo for [a droplet](https://www.digitalocean.com/products/droplets/?refcode=5fb69d9c62e4) and $5/mo for [Spaces](https://www.digitalocean.com/products/spaces/?refcode=5fb69d9c62e4) (their S3 storage) and be done. That's $10/mo for 250GB of storage and 1TB of bandwidth: more than enough for any number of websites.



