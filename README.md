# Some basics about this test

To make it work, three repository secrets should be configured.

1. `REPO_BEARER_TOKEN` with a value of the
 [Github personal access token for your repository](https://docs.github.com/en/enterprise-server@3.4/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token)
2. `SLACK_BOT_OAUTH` a bot OAuth token for slack notification.
I use `xoxb-684410959671-1628892673456-10zfFO1WHrHLKMAkDAGRlahh` for my own slack workplace.
Create your own slack workplace and bot OAuth token to avoid spaming my slack workplace - but for a single test you may use mine.
3. `SLACK_CHANNEL` channel name, in my case it is `random`

## Other moments

If you use different main branch, change line 20 of `sfdxManualBuild.yml` that contains code

`/commits?sha=main`

to

`/commits?sha=$yourBranch`