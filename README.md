# zaia.cz redirect

Fallback for the old zaia.cz domain after the rename to Keliqo (see the root README). Contents of a separate GitHub Pages
repo (proposed `zcloudcz/zaia-redirect`): GitHub Pages serves `404.html` for every unknown path, so one file sends every
zaia.cz address to the same path on keliqo.com.

Prefer a server-side `301` redirect at the zaia.cz DNS/hosting provider (same path and query) if it offers one: search
engines move rankings faster with a real 301 than with this JavaScript redirect. Use this repo only if it does not.
Publish it only after `web-aia` serves keliqo.com (its CNAME no longer says zaia.cz), otherwise GitHub refuses the domain.
