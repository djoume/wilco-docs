---
title: github_pr_approve
parent: Actions
grand_parent: Building Your Quest
nav_order: 6
---

# github_pr_approve

Category: Github
Description: Approve the PR and add comment on behalf of a bot.
Type: Action

## Description

**Type**: Action

Approve the PR and add comment on behalf of a bot

## Params

- **message:** The comment text
    
    [Text Formatting]
    

## Result

No additional info is added to the global payload outputs.

## Usage Example

```yaml
do:
- actionId: github_pr_approve
  params:
    message: "Nailed it! Excellent job @${user.githubuser}! You can now merge the PR."
```

The `github_pr_approve` action is used to approve the PR and let user know he should merge it. The message is sent on behalf of the bot `keen`

## Relevant Triggers

- `github_pr_lifecycle_status`

[Text Formatting]: {% link docs/building-your-quest/writing-quest-texts/text-formatting.md %}