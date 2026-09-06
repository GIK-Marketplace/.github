# GIK Marketplace

This repository holds the public organization profile for
[github.com/GIK-Marketplace](https://github.com/GIK-Marketplace).

| What | Where |
|---|---|
| Profile page shown on the org home | [`profile/README.md`](profile/README.md) |
| Org settings (description, website, location) | [`org-profile.json`](org-profile.json), applied with [`scripts/apply-org-profile.sh`](scripts/apply-org-profile.sh) |

## Organization settings

GitHub keeps an organization's description, website, and location in org
settings rather than in a repository, so this repo records the intended values
and ships a script that applies them.

| Field | Value |
|---|---|
| Display name | GIK Marketplace |
| Description | Moving at the Speed of Need. A free marketplace that matches corporate surplus to verified nonprofit needs for disaster relief and community response. |
| Website | https://gik.org |
| Location | Grand Rapids, MI |

To apply, an org owner runs the following from a machine with an authenticated
[GitHub CLI](https://cli.github.com):

```sh
./scripts/apply-org-profile.sh --dry-run   # preview
./scripts/apply-org-profile.sh             # apply
```

Edit `org-profile.json` first when the values need to change, then re-run the
script so the repo and the org settings stay in step.
