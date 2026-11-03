# Medill Solutions Journalism Hub Social Media Assets

A one-page website where colleagues can download a graphic and videos for the
**Reporting Under Pressure: State of the Craft** survey and copy ready-to-post
captions. It's built to run on **GitHub Pages** (free hosting from GitHub).

Survey link: https://www.medill.school/state-of-the-craft · Closes Monday, Nov. 23, 2026

---

## What's in this folder

```
medill-social-assets/
├── index.html                  ← the web page (intro, how-to, downloads, captions)
├── README.md                   ← this file
├── .nojekyll                   ← tells GitHub to serve files as-is (keep it)
└── assets/
    ├── images/
    │   ├── state-of-the-craft-1200x900.png        ← social graphic
    │   └── instagram-post.png                     ← Instagram post, 1080 × 1350
    └── video/
        ├── state-of-the-craft-video-1080x1350.mp4 ← Video 1, captioned (15 MB)
        ├── video-poster.jpg                       ← still frame shown before Video 1 plays
        (video-2.mp4 goes here later — see Part 2)
```

Keep the folder structure exactly as it is. The page looks for files by these
names and paths.

> **About `.nojekyll`:** files starting with a dot are hidden by default on Mac
> and Windows. It's an empty file and the site works without it, so if it gets
> left behind, don't worry.

---

## Part 1: Put the site on GitHub (no coding, all in the browser)

You need a free GitHub account. Sign up at https://github.com/signup if you
don't have one.

### Step 1. Create a repository

1. Sign in to https://github.com.
2. Click the **+** in the top-right corner, then **New repository**.
3. **Repository name:** `state-of-the-craft` (or any name; it becomes part of
   your web address).
4. **Description (optional):** `Medill Solutions Journalism Hub Social Media Assets`
5. Choose **Public**. (GitHub Pages is free only for public repositories on a
   free account.)
6. Leave the other boxes unchecked. Click **Create repository**.

### Step 2. Upload the files

You'll upload **three things in one go**: `index.html`, `README.md` and the
`assets` folder. Keep the `assets` folder in one piece: don't open it and
don't pull the files out of it. GitHub keeps its folders and files inside.
Nothing gets dragged *into* `index.html`; the page finds the files on its own.

1. Unzip `medill-social-assets.zip`. You'll get a folder called
   `medill-social-assets`.
2. Open that folder. Inside it are exactly three items (plus a hidden
   `.nojekyll` file you can ignore):

   ```
   assets        ← a folder; leave it closed
   index.html
   README.md
   ```

3. In your browser, on the new, empty repository page, click the link
   **uploading an existing file**. (If you don't see it: **Add file → Upload
   files**.)
4. Back in the `medill-social-assets` folder, select all three items
   (**Cmd+A** on a Mac, **Ctrl+A** on Windows). Drag them together onto the
   GitHub page where it says "Drag files here."
   - Drag the three items, **not** the outer `medill-social-assets` folder.
     If you drag the outer folder, everything lands one level too deep and the
     site won't load.
5. Wait until the list shows every file, including
   `assets/video/state-of-the-craft-video-1080x1350.mp4` (the 15 MB video
   takes a moment).
6. At the bottom, under **Commit changes**, type a short note such as
   `Add social assets page` and click **Commit changes**.

**Check:** the repository's main page should list `assets`, `index.html` and
`README.md`. Click into `assets` and you should see `images` and `video`
folders with the files inside.

### Step 3. Turn on GitHub Pages

1. In the repository, click **Settings** (top menu, gear icon).
2. In the left sidebar, click **Pages**.
3. Under **Build and deployment → Source**, choose **Deploy from a branch**.
4. Under **Branch**, choose **main** and folder **/ (root)**. Click **Save**.
5. Wait 1–3 minutes, then refresh the Settings → Pages screen. A box will say
   **"Your site is live at …"** with your address, which will look like:

   ```
   https://YOUR-GITHUB-USERNAME.github.io/state-of-the-craft/
   ```

6. Open it and check: the graphic shows, the video plays, the **Download** and
   **Copy caption** buttons work.

That's the link to send to colleagues.

### If the upload went wrong

- **You see one folder called `medill-social-assets` instead of the three
  items:** the outer folder was dragged. Delete the repository (Settings →
  scroll to the bottom → **Delete this repository**), create it again and
  redo Step 2.
- **`index.html` is there but the `assets` folder isn't:** your browser
  dropped the folder. Click **Add file → Upload files** and drag just the
  `assets` folder onto the page in Chrome or Edge. Clicking "choose your
  files" won't work for this, because the file picker can't upload folders.

---

## Part 2: Adding Video 2 later (and replacing the Instagram post)

The Download section has a tile reserved for **Video 2**. It shows a striped
"Coming soon" box until its file exists. (The Instagram post is already in
place; to swap it for a new version, upload a file with the same name.) Once you upload
the file with the right name, the tile fills itself in with a preview, the
file details and a working **Download** button. You don't need to edit any code.

| Tile | Upload to folder | File name (exactly, all lowercase) | Recommended format |
|---|---|---|---|
| Video 2 | `assets/video` | `video-2.mp4` | MP4 (H.264), 1080 × 1350 (4:5) or 1080 × 1920 (9:16), under 25 MB |
| Video 2 cover image (optional) | `assets/video` | `video-2-poster.jpg` | JPG still from the video, shown before it plays |
| Instagram post | `assets/images` | `instagram-post.png` or `instagram-post.jpg` | 1080 × 1350 (4:5) or 1080 × 1080 |

**To upload:**

1. In your repository, click into the folder (for example **assets**, then **video**).
2. Click **Add file → Upload files**, drag in the file, then click **Commit changes**.
3. Wait a minute or two, then reload the site. On a phone, you may need to
   close and reopen the tab.

**Optional: a description for Video 2.** Video 1 has a "Suggested description"
people can copy for accessibility. To add one for Video 2, open `index.html`,
click the pencil icon, find `data-ready="` and replace the sentence inside the
quotation marks with a one-line description of the video. That text appears
under Video 2 once the video is uploaded.

> If your video app exports `.mov` or `.MP4`, rename it to `video-2.mp4`
> (lowercase). If it's a `.mov`, export it again as MP4 first: iPhones and
> most browsers play MP4 reliably.

---

## Making other changes

**Edit text on the page** (a caption, the intro, a date):

1. In the repository, click `index.html`.
2. Click the **pencil icon** (Edit this file) at the top right of the file.
3. Use **Ctrl+F / Cmd+F** to find the words you want to change. Change only
   the words between the tags (the parts that aren't inside `< >`).
4. Click **Commit changes**. The live site updates within a couple of minutes.

**Replace the graphic or video:** upload a new file with **the exact same file
name** into the same folder (`assets/images` or `assets/video`). GitHub will
replace the old one. If you change a file name, you'd also need to update it
in `index.html`.

**File-size limits:** GitHub's web uploader accepts files up to **25 MB** each.
The current video is 15 MB. If a future video is bigger, export it at a lower
bitrate or use GitHub Desktop (which allows up to 100 MB).

**After the survey closes:** you can leave the page up as a record, or go to
**Settings → Pages** and click **Unpublish site**.

---

## Checklist before you share the link

- [ ] Page loads at your `github.io` address
- [ ] Graphic and Video 1 download on a computer
- [ ] Video downloads on a phone and can be saved to Photos
- [ ] "Copy caption" works (paste into a note to check)
- [ ] Every caption's link reads `www.medill.school/state-of-the-craft`
- [ ] **@MedillSchool** confirmed as the right handle on each platform
- [ ] Instagram post shows and downloads
- [ ] Video 2 uploaded (or the "Coming soon" tile is OK for now)

---

## What the page tells colleagues

The page is laid out as a bold poster in four numbered sections — 01 Why,
02 How, 03 Download, 04 Copy. It walks people through sharing in four steps (take the survey,
download an asset, copy a caption, post and pass it on), with separate
download tips for computers, iPhone/iPad and Android. It also reminds them to
check the @MedillSchool handle on each platform and that Instagram links
aren't clickable in captions ("link in bio" instead).

Each caption has a one-tap **Copy caption** button and a character count; the
short caption is flagged as fitting X (280), Bluesky (300) and Threads (500).
Each asset has suggested alt text that colleagues can copy for accessibility.
