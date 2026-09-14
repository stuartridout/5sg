# 5sg

The new owners' welcome-home manual, published via GitHub Pages.

`index.html` is the whole site: a single password-locked page. It's
built from an encrypted blob, so this repo can be public without
exposing what's inside - even the full commit history gives nothing
away.

The readable source, and the script that builds `index.html`, live in
the private `dev-hq` repo under `5sg-src/` (kept there deliberately,
see that folder's README for why). To update the manual, edit it there
and re-run the build script, which writes the new `index.html` straight
into this checkout.

## Hosting

Settings → Pages → Deploy from a branch → `main` / root. The page is
then at `https://stuartridout.github.io/5sg/`.

The password lock keeps the page off search engines and away from
casual visitors. It isn't a vault: a short password can be guessed
offline by anyone determined enough who downloads the page. Fine for a
house manual, not for anything you'd mind a stranger eventually reading.
