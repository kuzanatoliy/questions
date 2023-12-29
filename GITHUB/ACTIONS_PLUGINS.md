# Actions plugins

<details>
  <summary>What is a checkout action?</summary>

This action checks out your repository under $GITHUB_WORKSPACE, so your workflow can access.

It is possible to use following params:

| Name                      | Description                                                                                                                                                                               | Default                  |
| ------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------ |
| repository                | Repository name with owner                                                                                                                                                                | ${{ github.repository }} |
| ref                       | The branch, tag or SHA to checkout. When checking out the repository that triggered a workflow                                                                                            | Default branch           |
| token                     | Personal access token (PAT) used to fetch the repository                                                                                                                                  | ${{ github.token }}      |
| ssh-key                   | SSH key used to fetch the repository                                                                                                                                                      |                          |
| ssh-known-hosts           | Known hosts in addition to the user and global host key database                                                                                                                          |                          |
| ssh-strict                | Wheter to perform strict host key checking                                                                                                                                                | true                     |
| persist-credentials       | Whether to configure the token or SSH key with the local git config                                                                                                                       | true                     |
| path                      | Relative path under $GITHUB_WORKSPACE to place the repository                                                                                                                             |                          |
| clean                     | Wheter to execute `git clean -ffdx && git reset --hard HEAD` before fetching                                                                                                              | true                     |
| filter                    | Partially clone against a given filter. Overrides sparse-checkout if set                                                                                                                  | null                     |
| sparse-checkout           | Do a sparse checkout on given patterns                                                                                                                                                    | null                     |
| sparse checkout-cone-mode | Specifies whether to use cone-mode when doing a sparse checkout                                                                                                                           | true                     |
| fetch-depth               | Number of commits to fetch                                                                                                                                                                | 1                        |
| fetch-tags                | Whether to fetch tags, even if fetch-depth > 0                                                                                                                                            | false                    |
| show-progress             | Whether to show progress status output when fetching                                                                                                                                      | true                     |
| lfs                       | Whether to download Git-LFS files                                                                                                                                                         | false                    |
| submodules                | Whether to checkout submodules: `true` to checkout submodules or `recursive` to recursively checkout submodules.                                                                          |
| set-safe-directory        | Add repository path as safe.directory for Git global config by running `git config --global --add safe.directory <path>`                                                                  | true                     |
| github-server-url         | The base URL for the GitHub instance that you are trying to clone from, will use environment defaults to fetch from the same instance that the workflow is running from unless specified. |                          |

[More >>](https://github.com/actions/checkout)

</details>
