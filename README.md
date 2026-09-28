# Oskeriy.github.io

Developer website for **APP2GO**, served at <https://oskeriy.github.io>.

Its main job is to host `app-ads.txt` at the **root** of the domain, which is
the only place Google AdMob's crawler looks:

    https://oskeriy.github.io/app-ads.txt

## Files

| File           | Purpose                                                        |
| -------------- | -------------------------------------------------------------- |
| `app-ads.txt`  | AdMob publisher authorization (IAB Tech Lab app-ads.txt v1.0).  |
| `index.html`   | Landing page — the developer website listed on Google Play.     |
| `terms/index.html` | Terms of Service for Magnifier, at <https://oskeriy.github.io/terms/>. |
| `.nojekyll`    | Serve files verbatim, skipping the Jekyll build step.           |

## Notes

- The Google Play developer website must be entered as `https://oskeriy.github.io`
  (exactly — no trailing path), or the crawler will look at a different domain.
- After editing `app-ads.txt`, allow a few minutes for GitHub Pages to redeploy
  before re-running the check in AdMob.
- The privacy policy lives in a separate repo and is unaffected:
  <https://oskeriy.github.io/projects_privacy_policy/>
