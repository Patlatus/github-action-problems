# Some basics about this test

To make it work, three repository secrets should be configured.

1. `REPO_BEARER_TOKEN` with a value of the
 [Github personal access token for your repository](https://docs.github.com/en/enterprise-server@3.4/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token)
2. `SLACK_BOT_OAUTH` a bot OAuth token for slack notification.
It is bad idea to post secret in the readme file since it is automatically blocked by slack.
Create your own slack workplace and bot OAuth token.

3. `SLACK_CHANNEL` channel name, in my case it is `random`

## Other moments

If you use different main branch, change line 20 of `sfdxManualBuild.yml` that contains code

`/commits?sha=main`

to

`/commits?sha=$yourBranch`
