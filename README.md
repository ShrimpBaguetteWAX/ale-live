# ale-live

Production build target for the Alien Legends frontend.

**There is no source code here.** This repository holds nothing but the
built site, published by CI from
[`ShrimpBaguetteWAX/ale`](https://github.com/ShrimpBaguetteWAX/ale). Every
file on the publishing branch is generated output — editing anything here is
undone by the next release.

## How a release gets here

Work happens on `main` in `ale`, which publishes continuously to
<https://new.alienlegends.io> — the preview site. When a version there is
judged good, `live` in `ale` is fast-forwarded to that commit, and CI builds
that exact tree and pushes the result to this repository.

Fast-forward only, deliberately: nothing can reach production that was not
running on the preview site first.

## Status

Not yet serving. `alienlegends.io` and `www.alienlegends.io` still point at
the existing site and stay there until the cut-over is called. Until then
this repository has no Pages site and no custom domain attached.
