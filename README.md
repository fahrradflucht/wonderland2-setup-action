# wonderland2-setup-action
A GitHub action to setup wl2 cli in your workflow

## How to use

```yaml
- name: Configure WL2
  uses: Jimdo/wonderland2-setup-action@main
  with:
    cli-version: latest
    environment: prod

- name: Deploy to Wonderland 2
  run: wl2 deploy
```
