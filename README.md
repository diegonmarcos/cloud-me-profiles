# cloud-me-pub-profiles-___

Registry index for the cloud-me-pub-profiles family (company and profile sites) - same model as `CG-___`, `Fin-CM-___` and `cloud-___`. This repo is an INDEX, not a container: it holds `repos.json` (the registry, a subset of _git-repos-master/repos.json), `clone.sh` (pick which repos to have locally) and one committed relative symlink per member (`<member> -> ../<member>`); the actual clones live as siblings in `~/git/`.

## Members

- [cloud-me-pub-profiles-leaf.y](https://github.com/diegonmarcos/cloud-me-pub-profiles-leaf.y) - Leaf.y company site (/leafy/)
- [cloud-me-pub-profiles-nexus.z](https://github.com/diegonmarcos/cloud-me-pub-profiles-nexus.z) - Nexus.z company site (/nexus/)
- [cloud-me-pub-profiles-stark.x](https://github.com/diegonmarcos/cloud-me-pub-profiles-stark.x) - Stark.x company site (/stark/)
- [cloud-me-pub-profiles-prf-prs](https://github.com/diegonmarcos/cloud-me-pub-profiles-prf-prs) - profile sites: b_Profiles and c_Circus/myAstro
- [cloud-me-pub-profiles-_lnktree](https://github.com/diegonmarcos/cloud-me-pub-profiles-_lnktree) - Linktree sources

## Usage

```
./clone.sh                list what exists and what does not
./clone.sh <name>...      clone those, then link them
./clone.sh --all          clone every member
./clone.sh --link         relink whatever is already cloned
./clone.sh --relink       rewrite every link from the registry
./check-repos-sot.sh      verify repos.json against _git-repos-master
```

`repos.json` is a SUBSET of `~/git/_git-repos-master/repos.json` (the superset index of every repo this account owns): identical name/url/private/doc fields, checked by `./check-repos-sot.sh`.
