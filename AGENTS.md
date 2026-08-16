# PiPCounter Development Instructions

## Project overview

PiPCounter is a small web application intended to be hosted on GitHub Pages.

The application provides a counter that can be used from an iPhone browser,
including Picture-in-Picture related functionality.

The main development file is:

- `devmain/index.html`

## Editable files

All implementation changes must be made only inside:

- `devmain/`

Do not modify files outside `devmain/`.

## Read-only directories

The following directories may be inspected when necessary, but must never be modified:

- `.git/`
- `.github/`
- `.codex/`
- `temp/`

`temp/` contains historical versions of `index.html`.
Files in `temp/` may be referenced for comparison, but must not be changed,
deleted, renamed, or created.

## Git operations

GitHub operations are performed manually by the user.

Do not perform:

- `git add`
- `git commit`
- `git push`
- `git pull`
- `git merge`
- `git rebase`
- branch creation or deletion
- tag creation or deletion

Read-only Git commands such as the following are allowed when useful:

- `git status`
- `git diff`
- `git log`

## Development policy

When asked to implement or modify functionality:

1. Inspect `devmain/index.html`.
2. Refer to files under `temp/` only when historical comparison is useful.
3. Make changes only under `devmain/`.
4. Do not create backup files in `temp/`.
5. Do not publish or deploy the project.
6. Do not modify GitHub Actions or GitHub Pages configuration.
7. Report the files changed after completing the task.

## Application constraints

The application is intended to run as a static GitHub Pages site.

Prefer:

- HTML
- CSS
- JavaScript
- browser-native APIs

Avoid introducing:

- server-side components
- build systems
- package managers
- external dependencies

unless explicitly requested by the user.

Maintain compatibility with Chrome on iPhone as a primary target.
