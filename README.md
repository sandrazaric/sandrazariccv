**To deploy to GitHub Pages:**

1. Run `npm run build` - this creates an `out/` folder with static HTML/CSS/JS
2. Push the `out/` folder contents to your GitHub repo's `gh-pages` branch, or configure GitHub Pages to serve from the `out/` folder
3. If your repo is at `username.github.io/repo-name` (not the root), uncomment the `basePath` line in `next.config.mjs` and set it to `/your-repo-name`


The images are already set to `unoptimized: true`, which is required for static export since Next.js Image Optimization needs a server.

To serve at `https://sandrazaric.github.io` (root), you need to:

1. **Rename your repository** to exactly `sandrazaric.github.io` (not `sandrazariccv`)
2. Push the static `out/` folder contents to the `main` or `gh-pages` branch
3. In GitHub repo settings > Pages, set the source to the correct branch


GitHub Pages only serves from the root domain when the repository name matches the pattern `username.github.io`. Any other repository name will automatically be served at `username.github.io/repo-name`.

The code is already configured correctly for root deployment (no basePath). You just need to rename the repository on GitHub from `sandrazariccv` to `sandrazaric.github.io`.

To start locally:
npm install
npm run build
npx serve@latest out