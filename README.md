# public

public repo でしか検証できないものを扱う。

## github actions environments

任意のブランチ名でプッシュすると、provision の job が走る。
そのあと approval が求められ、approve すると、deploy-development の job が走る。

### ref

<https://docs.github.com/en/actions/reference/environments>

> Environments, environment protection rules, and environment secrets are available in public repositories for all products and in private repositories for GitHub Enterprise.

<https://devblogs.microsoft.com/devops/i-need-manual-approvers-for-github-actions-and-i-got-them-now/#how-do-i-do-this>

→ ソース参考

<https://github.com/actions/github-script#comment-on-an-issue>

→ を使って approval を待っている際に PR に CI の output を post するのもよかろう。
