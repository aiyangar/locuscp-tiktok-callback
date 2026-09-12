# locuscp-tiktok-callback

Static callback page for the one-time TikTok OAuth authorization of
[locuscp](https://github.com/aiyangar/locuscp) (its `tiktok-setup` subcommand).

TikTok requires the OAuth `redirect_uri` to be an absolute, static HTTPS URL,
so this page is served by GitHub Pages at
`https://aiyangar.github.io/locuscp-tiktok-callback/`. It only reads the
`code` and `state` query parameters out of the URL and displays them so they
can be pasted back into the terminal running `tiktok-setup`. Nothing is sent
anywhere.

`index.html` is a verbatim copy of `docs/tiktok-oauth-callback.html` in the
locuscp repo; change it there first, then copy it here.
