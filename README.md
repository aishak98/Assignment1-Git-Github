# Task 2 – Git Workflow Practice

## Branch Overview
- **main**: Stable production branch
- **dev**: Development/integration branch
- **feature1**: Feature branch that will be updated from dev and merged
- **feature2**: Feature branch that will be rebased onto dev
- **feature3**: Feature branch with messy commits that will be squashed and rebased
- **hotfix**: Critical fix branch to be cherry-picked into main
- **documentation**: Notes and explanations for Task 2

## Planned Git Strategies
- Merge dev into feature1
- Rebase feature2 onto dev
- Squash + rebase feature3
- Cherry-pick hotfix into main

## Differences
- merge: combines histories, creates a merge commit when needed (good for shared branches)
- rebase: rewrites commits onto a new base to make history linear (avoid on shared branches)
- squash: turns many commits into 1 (cleaner history before merging)
- cherry-pick: copies a single commit to another branch (great for hotfixes)

## What I observed in history
- feature1: merge workflow (merge dev into feature, then merge into dev)
- feature2: rebase workflow (linear history, conflicts resolved during rebase)
- feature3: squashed multiple commits into one before rebasing/merging (cleanest)

## When to use what
- Merge: team/shared branches
- Rebase: local cleanup before PR
- Squash: clean PR history
- Cherry-pick: urgent fix onto main + bring back to dev

## Notes
This README documents the Git strategies used in Task 2 and why each was chosen.
