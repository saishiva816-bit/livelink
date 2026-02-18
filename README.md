# LIVE player

This site contains a single self-contained `index.html` (copied from `player.html`) which runs a Shaka-based player.

Quick local test:

```powershell
cd D:\Projects\LIVE
python -m http.server 8080
# then open http://localhost:8080/index.html
```

Deploy to Netlify (drag & drop):
- Zip the `D:\Projects\LIVE` folder or drag & drop into the Netlify Sites "New site from git / drag & drop" panel.

Deploy with Netlify CLI (recommended for production):

```powershell
# install CLI if needed
npm install -g netlify-cli

# login and deploy
netlify login
cd D:\Projects\LIVE
netlify deploy --prod --dir=.
```

Notes:
- Netlify will serve `index.html` as the root page.
- If your stream is geo-restricted or requires authentication, Netlify cannot bypass that. Consider using a server-side proxy (Netlify Functions) or a public HLS/DASH stream.
"# livelink" 
"# livelink" 
