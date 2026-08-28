# github-actions

| `prevent-branches-without-jira-ticket`               |  Prevent pull requests from branches without a Jira ticket key.

---
### prevent-branches-without-jira-ticket

Requires a branch name to contain a Jira ticket key. The rest of the branch name is unrestricted, so names such as `feature/RE-1234-add-login` and `bugfix/REBNCRDMP-57` are valid. The accepted key formats are `RE-{number}` and the legacy `REBNCRDMP-{number}`.

Full path:
```
we-eisos/tm-redexpert-actions/prevent-branches-without-jira-ticket
```

Use it in a pull-request workflow after checkout:

```workflow
steps:
  - uses: we-eisos/tm-redexpert-actions/prevent-branches-without-jira-ticket@v1
```

It has no input and output parameters.