# Updating the site (all from the GitHub website, no coding)

Open a file in the `data` folder > pencil icon > edit > *Commit changes*. The site refreshes about a minute later.

| What | File |
|---|---|
| Musicals / Audios / Plays you have | `data/musicals.txt`, `data/audios.txt`, `data/plays.txt` |
| Status, Updated date, Email, Reddit | `data/site.txt` |
| Wishlist | `data/wishlist.txt` |
| Contact & Rules page text | `data/rules.txt` |
| Format help (dates, tags, posters, Added) | `data/_guide.txt` |

**Posters:** open the `image` folder > *Add file > Upload files*. Name each picture after the show (`falsettos.jpg`, `Dear Evan Hansen.png`).
**Header photo:** replace `image/header.jpg` (keep that name).

# Moving from the old single file (data/collection.txt)

The new data files come empty, so uploading them changes nothing for visitors: the site keeps using `data/collection.txt` until you fill in the new files.
1. Copy the shows under `# Musicals` into `data/musicals.txt`, the ones under `# Recordings` (now called Audios) into `data/audios.txt`, and `# Plays` into `data/plays.txt` (move all three, then the old file is ignored).
2. Copy the Updated / Status / Email / Reddit lines into `data/site.txt`.
3. Delete `data/collection.txt`.

# Adding entries with one tap (add.html)

Bookmark `https://YOUR-SITE/add.html` (it isn't linked anywhere on the site). Pick Collection or Wishlist, fill in what you know, optionally choose a poster, and press **Add & save to GitHub**. It writes the entry in the right data file (under the right `# heading` for the wishlist), uploads the poster to the `image` folder, sets `Added:` to today and refreshes `Updated:` in `data/site.txt` when that line exists.
First time only: open the *GitHub connection* box and paste a fine-grained token that has **Contents: Read and write** on this one repo (steps are on the page). The token stays in your browser only. Anyone who has it can change that repo, so don't share it or put it in any file. Move your old entries into the new files before using the page (see above).

# One-time setup

1. Create a GitHub repo, upload everything in this folder (*Add file > Upload files*).
2. *Settings > Pages > Deploy from a branch > main / (root)*.
3. Emails: get a free access key at https://web3forms.com and paste it into `collection.html` and `contact.html`, where it says `accessKey`. The key is safe to be public; it only lets people send *to you*.
