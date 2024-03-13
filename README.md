# [GitHub Stats Visualization : React Theme](https://github.com/jk1635/github-stats-react-theme)

<a href="https://github.com/jk1635/github-stats-react-theme">

![](https://github.com/jk1635/github-stats-react-theme/blob/main/generated/overview.svg)
![](https://github.com/jk1635/github-stats-react-theme/blob/main/generated/languages.svg)

</a>

> This repository is a extensions of the repo [jstrieb/github-stats](https://github.com/jstrieb/github-stats).

## Installation

<!-- TODO: Add details and screenshots -->

1. Create a personal access token (not the default GitHub Actions token) using
   the instructions
   [here](https://docs.github.com/en/github/authenticating-to-github/creating-a-personal-access-token).
   Personal access token must have permissions: `read:user` and `repo`. Copy
   the access token when it is generated – if you lose it, you will have to
   regenerate the token.
2. Click [here](https://github.com/jk1635/github-stats-react-theme/fork) to create a
   copy of this repository.
3. If this is the README of your fork, click [this
   link](../../settings/secrets/actions) to go to the "Secrets" page.
   Otherwise, go to the "Settings" tab of the newly-created repository and go
   to the "Secrets" page (bottom left).
4. Create a new secret with the name `ACCESS_TOKEN` and paste the copied
   personal access token as the value.
5. It is possible to change the type of statistics reported.
   - To ignore certain repos, add them (in owner/name format e.g.,
     `username/github-stats-react-theme`) separated by commas to a new secret—created as
     before—called `EXCLUDED`.
   - To ignore certain languages, add them (separated by commas) to a new
     secret called `EXCLUDED_LANGS`. For example, to exclude HTML and TeX you
     could set the value to `html,tex`.
   - To show statistics only for "owned" repositories and not forks with
     contributions, add an environment variable (under the `env` header in the
     [main
     workflow](https://github.com/jk1635/github-stats-react-theme/blob/main/.github/workflows/main.yml))
     called `EXCLUDE_FORKED_REPOS` with a value of `true`.
6. Go to the [Actions
   Page](../../actions?query=workflow%3A"Generate+Stats+Images") and press "Run
   Workflow" on the right side of the screen to generate images for the first
   time. The images will be periodically generated every hour, but they can be
   manually regenerated by manually running the workflow.
7. Check out the images that have been created in the [`generated`](generated)
   folder.
8. To add your statistics to your GitHub Profile README, copy and paste the following 
   lines of code into your markdown content. Change the `username` value to your GitHub 
   username.
   ```md
   ![](https://github.com/username/github-stats-react-theme/blob/main/generated/overview.svg)
   ```
   ```md
   ![](https://github.com/username/github-stats-react-theme/blob/main/generated/languages.svg)
   ```
9. Link back to this repository so that others can generate their own
   statistics images.
10. Star this repo if you like it!

## Related Projects

- [jstrieb/github-stats](https://github.com/jstrieb/github-stats)
- [rahul-jha98/github-stats-transparent](https://github.com/rahul-jha98/github-stats-transparent)
- [anuraghazra/github-readme-stats](https://github.com/anuraghazra/github-readme-stats)
