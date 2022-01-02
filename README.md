# notes-source EXAMPLE FILES (public)

For instructions on how to use Hugo and GitHub Pages to host your content for free, see [Create and Host a Blog for Free (~1 hour)](https://denisecase.github.io/notes/post/2022-01-01-publish/)).

The linked article shows how to create:

- a private repo (e.g., [notes-source](https://github.com/denisecase/notes-source))
- a public repo (e.g., [notes](https://github.com/denisecase/notes))

The private repo is what we use while writing and developing the site. The public repo gets automatically generated using Hugo and GitHub Actions. The public repo hosts the site for free using GitHub Pages.

-----

This repo is not part of the process - it just illustrates files found in the private `notes-source` folder described in the article.

The GitHub repo [Actions](https://github.com/denisecase/notes-source-example/actions) will not work - the [deploy.yml](https://github.com/denisecase/notes-source-example/blob/main/.github/workflows/deploy.yml) file needs to replace the line:

  ```
  personal_token: ${{ secrets.PERSONAL_TOKEN }}
  ```

with the actual value. The secret is only available in the private repo, [notes-source](https://github.com/denisecase/notes-source) where this line looks more like:

  ```
  personal_token: ghp_abcdefghijklmnopq...
  ```
