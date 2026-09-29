# Personal blog — Hugo

## Preview
```sh
hugo server -D
```
Open the URL printed by Hugo.

## Personalize
- Edit `hugo.toml`: name, title, introduction, description, and email.
- Edit `content/about.md` and `content/contact.md`.
- Each course has its own folder under `content/blog/`. No sample posts are included.

## Write
```sh
hugo new content --kind blog blog/bcv/my-first-post.md
```
Edit the new Markdown file and set `draft: false` when ready. Replace `bcv` with the course folder below. The post will appear automatically on its course page.

| Folder | Course |
| --- | --- |
| `cg` | Computer Graphics |
| `bcv` | Basic Computer Vision |
| `hci` | Human-Computer Interface |
| `ai` | Artificial Intelligence |
| `acv3d` | Advanced Computer Vision & 3D Reconstruction |
| `sr` | Social Robotics |
| `collenv` | Collaborative Environments |
| `ar` | Augmented Reality |
| `vr` | Virtual Reality |
| `proj` | Transversal Project |

## Build
```sh
hugo --minify --cleanDestinationDir
```
The generated website is in `dist/`. Set `baseURL` to your final website URL before deploying it to your chosen host.

No theme downloads, Node.js, or external fonts are required. Navigation, article pages, pagination, RSS, and mobile layouts are included.

Reference: https://gohugo.io/documentation/

## GitHub Pages
1. Create a public repository named `my-blog` under the `Tims-ansu` account.
2. Upload this project's source files to its root, including `.github/workflows/hugo.yaml`. Do not upload `dist/` or `.openai/`.
3. Open **Settings → Pages** and set **Source** to **GitHub Actions**.
4. Open **Actions → Build and deploy Hugo → Run workflow** on `main`.
5. Once deployment succeeds, open `https://tims-ansu.github.io/my-blog/`.

Later pushes to `main` automatically rebuild the website. The workflow uses the actual Pages URL, so it also supports a normal project repository with a URL subpath.

Reference: https://gohugo.io/host-and-deploy/host-on-github-pages/
