---
icon: youtube
---

# Downloading YouTube Videos

## Using an App&#x20;

I prefer using [Stacher7](https://s7.stacher.io/), which is an open source GUI application built on top of yt-dlp, another open source project well known for allowing video and audio archiving.

Because Stacher7 is built on top of yt-dlp and ffmpeg packages, you may be prompted to install those command line packages.&#x20;

<figure><img src="../../.gitbook/assets/image (9).png" alt="" width="375"><figcaption></figcaption></figure>

### Requirements

1. Ensure there's a check mark in the top right.

<figure><img src="../../.gitbook/assets/image (13).png" alt="" width="563"><figcaption></figcaption></figure>

2. If there isn't a check, click on the bubble telling you to install yt-dlp, ffmpeg, or both. Follow the on-screen instructions. If you get errors downloading them from this menu, you can always check out [how to install them manually (archived version of article)](https://web.archive.org/web/20250304135513/https://www.spacebar.news/how-to-install-yt-dlp/#expand).

### How to Download a Video

1. Paste a URL into the field
2. Click "Best Av" or whatever button is next to the download button

<figure><img src="../../.gitbook/assets/image (10).png" alt="" width="375"><figcaption></figcaption></figure>

3. Select the desired format

<figure><img src="../../.gitbook/assets/image (11).png" alt="" width="375"><figcaption></figcaption></figure>

4. Click the download button! Wait a bit, and you'll have your file.

***



## Using the Command Line

If you prefer to use Terminal, you can download and [how to install yt-dlp and ffmpeg manually (archived version of article)](https://web.archive.org/web/20250304135513/https://www.spacebar.news/how-to-install-yt-dlp/#expand)

I use macOS, so I installed yt-dlp using the [Homebrew package manager](https://formulae.brew.sh/formula/yt-dlp#default). It's also available for  package managers on other operating systems (e.g. Chocolatey and apt). You can also use a direct download if you'd prefer to not use a package manager (idk why you would tho).

If you're using this method, I assume you can read the documentation [over at Github](https://github.com/yt-dlp/yt-dlp/) and have used a command line utility before.

Here's two quick commands to get you started:

### Download a Video

_Download the best mp4 video available, or the best video if no mp4 available:_

```
yt-dlp "video_url_here" -f "bv*[ext=mp4]+ba[ext=m4a]/b[ext=mp4] / bv*+ba/b"
```

### Download Audio Only

_Download the best audio file available, regardless of file format:_

```
 yt-dlp "video_url_here" --extract-audio --audio-quality 0
```







