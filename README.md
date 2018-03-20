# Hosted CI/CD scripts [![ci-cd.net](https://img.shields.io/badge/ci--cd.net-website-blue.svg)](http://ci-cd.net) [![GitHub](https://img.shields.io/badge/ci--cd.net-on_github-000000.svg)](https://github.com/omrilotan/ci-cd.net) [![](https://circleci.com/gh/omrilotan/ci-cd.net.svg?style=svg)](https://circleci.com/gh/omrilotan/ci-cd.net)

## webhook
<img width="422" alt="Webhook notification example" src="https://user-images.githubusercontent.com/516342/37597214-66cdc4ec-2b87-11e8-94a9-0830dc222d1a.png">

Using defaults: environment variable `$WEBHOOK` and template file `.webhook.json`:
```bash
curl ci-cd.net/webhook | bash
```

Use other values:
```bash
curl ci-cd.net/webhook | bash -s <CUSTOM_WEBHOOK_URL> <CUSTOM_JSON_FILE>
```

Example JSON (CircleCI finished job -> Slack webhook)
```json
{
  "attachments": [
    {
      "fallback": "$CIRCLE_PROJECT_REPONAME finished CI job",
      "color": "#27ae60",
      "author_name": "$CIRCLE_PROJECT_REPONAME",
      "author_link": "$CIRCLE_REPOSITORY_URL",
      "title": "CI workflow finished",
      "text": "Automated operation triggered by *$CIRCLE_USERNAME*",
      "mrkdwn_in": ["text"]
    }
  ],
  "channel": "#team-channel",
  "username": "CircleCI",
  "icon_emoji": ":robot_face:"
}
```
