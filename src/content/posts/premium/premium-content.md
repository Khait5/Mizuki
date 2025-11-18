---
title: "Exclusive Gallery Vault: Uncensored BDO & Once Human Albums"
published: 2025-11-25
description: Private access to high-resolution, uncensored fan art and renders of BDO and Once Human characters. Access granted for Premium Tier 3 users only.
encrypted: true
pinned: false
password: "123456"
tags: ["Exclusive", "NSFW", "Gallery", "BDO", "OnceHuman"]
category: "premium users"
draft: false
---

# 🔞 PREMIUM GALLERY VAULT

Welcome, Premium User. Below is the list of exclusive, uncensored media albums. These files are not hosted on the public site and require manual configuration for viewing.

---

## 🖼️ Available Albums List

| Album Name | Content Focus | Access Folder | Number of Images |
|---|---|---|---|
| **Black Desert: Dark Knight Renders** | Exclusive renders of Dark Knight outfits and poses. | `bdo-dk-vault` | 42 |
| **Once Human: Doll Custom Showcase** | Unique, high-detail customization of Doll characters. | `oh-doll-custom` | 35 |
| **BDO: Sorceress (Succ) Collection** | High-resolution art focusing on the Sorceress Succession class. | `bdo-sorc-succ` | 28 |
| **Cross-Game: Mixed Fan Art** | Various characters from both games in shared scenes. | `mixed-fanart-vol1` | 50 |

---

## 💾 Upload Location and Configuration

To make these albums accessible on your Astro site, you typically need to place the images in a specific directory structure and ensure your theme's gallery component can read them.

### 1. Image Upload Location

**You should create the album folders inside your static assets directory.**

Assuming your Astro project follows the standard structure:

* **Path:** `public/assets/galleries/`

**Action:** Place the image files for each album in the corresponding folder:

* `public/assets/galleries/bdo-dk-vault/`
* `public/assets/galleries/oh-doll-custom/`
* `public/assets/galleries/bdo-sorc-succ/`
* `public/assets/galleries/mixed-fanart-vol1/`

### 2. Gallery Component Usage

Your theme likely has a custom component for displaying these albums (e.g., `<Gallery />` or `<AlbumList />`). You would typically use this component in your Markdown or an Astro layout page, feeding it the folder path.

**Example (Inside an Astro page or component):**

```astro
---
import Gallery from '~/components/Gallery.astro';
---
<h1>Black Desert: Dark Knight Renders</h1>
<Gallery albumFolder="bdo-dk-vault" />