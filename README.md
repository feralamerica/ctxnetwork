# theclocktowerx.com — flat single-folder version

ALL FILES SIT AT THE REPO ROOT. No subfolders except the two workflow files.

## Upload (GitHub web, no folder dragging needed)
1. New public repo. Click "uploading an existing file".
2. Select ALL of these at once and drop them in:
   index.html, allyvia.html, CNAME, metrics.json, feeds.json, README.md
3. Commit.
4. The TWO workflow files must live in a special folder. For each one, click
   "Add file > Create new file", and type the filename EXACTLY as:
        .github/workflows/update-feeds.yml
   (typing the slashes makes GitHub create the folders). Paste the contents
   from update-feeds.yml. Repeat for .github/workflows/update-metrics.yml.

## Then
- Edit .github/workflows/update-feeds.yml: replace UCXXXX... with your @feralamerica YouTube channel ID.
- Settings > Pages > custom domain: theclocktowerx.com > Enforce HTTPS.
- Actions tab > run both workflows once.

## DNS (theclocktowerx.com)
- A @ 185.199.108.153 / .109.153 / .110.153 / .111.153
- CNAME www -> feralamerica.github.io
- delete the "WebsiteBuilder Site" A record.

## Adding the other 10 dossiers later
Each is a root-level file like cognitura.html, paxpoint.html, etc. Ask and they'll be generated flat.
