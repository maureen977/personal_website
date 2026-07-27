# shupingwu.com — personal website

Pages: `index.html` (Home), `research.html`, `cv.html` (embedded PDF preview).
Assets: `photo.jpg` (headshot), `cv.pdf` (current CV), `style.css`.

You can delete `IMG_2996.JPG` and `CV_ShupingWu_AOM.pdf` from this folder — they were the
originals, already resized/copied into `photo.jpg` and `cv.pdf`.

## Before publishing

1. **Google Scholar**: in `index.html`, replace `YOUR_SCHOLAR_ID` with your Scholar profile ID
   (or remove that link if you don't have a profile yet).
2. **CV updates**: overwrite `cv.pdf` whenever your CV changes, and update the
   "Last updated" date in `cv.html`.

## Design notes

- Mostly white and minimal; a fixed field of soft, slowly drifting gradient blobs sits behind
  the content (`.aurora` in `style.css`), with a fine grain overlay so it doesn't look synthetic.
- To change the palette, edit the four `.blob` colors and the `--accent` variables at the top of
  `style.css`. For a calmer background, lower `.aurora { opacity }` (currently 0.55).
- Motion is disabled automatically for visitors who prefer reduced motion.
- Headings use Instrument Serif (loaded from Google Fonts; falls back to Georgia offline).

## Deploying (GitHub Pages, free)

1. Create a GitHub repository (e.g., `website`).
2. Upload all files in this folder to the repository root.
3. Settings → Pages → Source: `main` branch, root folder. Save.
4. Settings → Pages → Custom domain: `www.shupingwu.com`; at your registrar, add a CNAME
   record for `www` pointing to `<username>.github.io`.

Netlify or Cloudflare Pages work the same way: drag the folder in, then connect the domain.
