---
title: Tractorbeam - Open source multi-tier website backups
layout: page
show_sidebar: false
hide_hero: true
---
## Open source multi-tier website backups

Tractorbeam is a Docker container that can back up your entire website from a variety of hosts to S3-compatible object stores like AWS S3, [DigitalOcean Spaces](https://www.digitalocean.com/products/spaces/?refcode=5fb69d9c62e4), Google Cloud Storage, Ceph Object Storage, and more.  All libraries and utilities are built in to the container, so there's nothing more you need.


## If your website's host already has backups, why do you need Tractorbeam?

Because your host’s backups are likely in the same place as your site. What if something happens to that data center? Your site and your backups might be compromised. It always makes good business sense to have off-site backups. [Tractorbeam can help you get there!](/support/)


## Using Tractorbeam

Run the single shot container on your own infrastructure, see [tractorbeam.ten7.com/setup](/setup/) for details.


## Capabilities

- **Tractorbeam does multi-tier backups daily, weekly and monthly**  
By default, Tractorbeam keeps seven daily backups, four weekly backups and twelve monthly backups.
- **Tractorbeam can write backups to any S3-compatible hosting provider**  
DigitalOcean, Amazon S3 and Google Cloud Storage are used tested and used in production.
- **Tractorbeam keeps a set number of backups**  
The value of backups decrease the older they get. Tractorbeam automatically prunes backups before uploading to S3.
- **Tractorbeam works with most hosts**  
If there's SSH access, Tractorbeam will most likely work for you. It backs up any files you configure as well as MySQL and MariaDB databases. [Pantheon](https://pantheon.io/) and [platform.sh](https://platform.sh/) is also supported and works out of the box.
- **Tractorbeam is free and open source, so you have complete ownership of and access to your backups**  
You only have to pay for the server Tractorbeam runs on, and the storage of the backups themselves.
- **Tractorbeam does not care which CMS you use**  
If you have SSH access to your site's files, and it uses MySQL or MariaDB, Tractorbeam will back it up. So, it works with Drupal, Wordpress, Expression Engine, custom PHP apps, Laravel and more. Need support? [Let us know how we can help!](/support.html)



## Cost

Zilch. Nothing. Nada. Free!

It's free to use Tractorbeam, **but you will need to pay to host your backups somewhere**. For example, if you were to use [Digital Ocean](https://m.do.co/c/5fb69d9c62e4), you could pay $5/mo for [a droplet](https://www.digitalocean.com/products/droplets/?refcode=5fb69d9c62e4) and $5/mo for [Spaces](https://www.digitalocean.com/products/spaces/?refcode=5fb69d9c62e4) (their S3 storage) and be done.

That's $10/mo for 250GB of storage and 1TB of bandwidth: more than enough for numerous websites.
