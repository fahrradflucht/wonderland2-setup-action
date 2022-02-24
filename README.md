# wonderland2-setup-action
A GitHub action to setup wl2 cli in your workflow

## How to use

Provide a github token with `repo` and `read:org` scopes and a valid ssh key for the same user.
After the setup step, you can use the `wl2` cli as needed. The example shows a deployment.

```yaml
- name: Configure WL2
  uses: Jimdo/wonderland2-setup-action@main
  with:
    wonderland-github-token: ${{ secrets.WONDERLAND_GITHUB_TOKEN }}
    bastion-key: ${{ secrets.WONDERLAND_SSH_KEY }}

- name: Deploy to Wonderland 2
  run: wl2 deploy
```
