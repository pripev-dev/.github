# `.github`

Organisation-level files for [`pripev-dev`](https://github.com/pripev-dev).

| Path | What it does |
|---|---|
| [`profile/README.md`](profile/README.md) | The organisation profile. Renders on the org page **only while this repository is public** – a private `.github` shows it to nobody. |
| [`CODE_OF_CONDUCT.md`](CODE_OF_CONDUCT.md) | Default for every repository in the org that does not carry its own. |
| [`CONTRIBUTING.md`](CONTRIBUTING.md) | Default contribution guide. |
| [`SECURITY.md`](SECURITY.md) | How to report a vulnerability or a privacy problem. |
| [`SUPPORT.md`](SUPPORT.md) | Where questions go. |
| [`.github/ISSUE_TEMPLATE/`](.github/ISSUE_TEMPLATE) | Default issue forms. The nested path is GitHub's, not a mistake. |
| [`.github/PULL_REQUEST_TEMPLATE.md`](.github/PULL_REQUEST_TEMPLATE.md) | Default pull request template. |
| `brand/` | Reserved. Logo, avatar and banners land here once the design system exists; there is deliberately no wordmark yet. |

## Two things worth knowing

**Default community health files follow visibility.** A private `.github` supplies
defaults to private repositories only; a public one supplies them to public
repositories only. While the whole org is private this repository serves the private
repos. When `cookbook-agent` goes public it stops inheriting from here unless this
repository is public too.

**Publishing this repository is a brand decision, not a housekeeping one.** It puts the
name and the pitch on a public page. `handbook/docs/legal/05` records a live EUTM,
PRIPEC, one consonant away in the same Nice classes. Read it before flipping.

Line endings are pinned to LF in [`.gitattributes`](.gitattributes) because GitHub
renders these files itself.
