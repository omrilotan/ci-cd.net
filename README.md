# Hosted CI/CD scripts [![ci-cd.net](https://img.shields.io/badge/ci--cd.net-website-blue.svg)](http://ci-cd.net) [![GitHub](https://img.shields.io/badge/ci--cd.net-on_github-000000.svg)](https://github.com/omrilotan/ci-cd.net) [![](https://circleci.com/gh/omrilotan/ci-cd.net.svg?style=svg)](https://circleci.com/gh/omrilotan/ci-cd.net)

## Using hosted shell scripts
Using a script with defaults
```
curl ci-cd.net/v1/<SCIRIPT> | sh
```

Passing arguments
```bash
curl ci-cd.net/v1/<SCRIPT> | sh -s <ARGUMENT_1> <ARGUMENT_2>
```

## TOC

| script | description
| --- | ---
| [webhook](#webhook) | Post (or Get) request to a webhook
| [git/user](#gituser) | **If missing**, configure git user
| [git/update](#gitupdate) | Commit changes if there are any changes to commit

# V1

## webhook

<img width="422" alt="Webhook notification example" src="https://user-images.githubusercontent.com/516342/37597214-66cdc4ec-2b87-11e8-94a9-0830dc222d1a.png">

> The webhook will execute a POST a JSON file to the specified address, or a GET request when no JSON file is found. It will use the shell to "process" the JSON file, so any environment variables included in the text will be transformed.

### Arguments
**No arguments** - Use environment variable `WEBHOOK` and `.webhook.json` file

| Argument | Role | Default
| --- | --- | ---
| 1 | webhook address | $WEBHOOK
| 2 | JSON to post | `.webhook.json`

> #### Example
> `curl ci-cd.net/v1/webhook | sh -s $MY_WEBHOOK ./.custom-webhook-message.json`

#### JSON Examples
CircleCI finished job -> Slack webhook
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

## git/user
> Configure git user

### Arguments
**No arguments** - Use user from last commit

| Argument | Role | Default
| --- | --- | ---
| 1 | webhook address | $WEBHOOK
| 2 | JSON to post | `.webhook.json`

> #### Example
> `curl ci-cd.net/v1/git/user | sh -s CI-CD ci-cd@gmail.com`

## git/update

<img width="624" alt="image" src="https://user-images.githubusercontent.com/516342/37645734-5cad4f7e-2c30-11e8-99ee-5d4462ee606b.png">

> Commit changes if there are any changes to commit. Then commit them upstream. This requires the environment holds push privileges, and a user has been configured (see [git/user](#gituser))


### Arguments
**No arguments** - Use a random commit message from [whatthecommit.com](https://whatthecommit.com/)

| Argument | Role | Default
| --- | --- | ---
| @ | commit message | random commit message

> #### Example
> `curl ci-cd.net/v1/git/update | sh -s Automated commit from CI`
