# webinar-compuware

# One time setup

1. Add `ADMIN_PASSWORD` and `XLR_LICENCE` (the license base64 encoded) variables in a `.env` file in the same folder as the `docker-compose.yml`, like so:
```
ADMIN_PASSWORD=

XLR_LICENSE=
```
1. Add to the `secrets.xlvals` in the `xlr` folder, adding the secret values obviously: 
```
# This file includes all secret values, and will be excluded from GIT. You can add new values and/or edit them and then refer to them using '!value' YAML tag

jira_url = 
jira_username = 
jira_password = 

xlrelease_password = 

ispw_password = 

sonar_Server_password = qocnU1-tabdik-fyjzin

```

1. Install Docker and do open up the TCP port [see here](https://redtalks.live/2017/05/26/redtalks-18-enabling-the-docker-tcp-api-in-aws/)

# Deploy to Amazon

1. `git clone https://github.com/xebialabs-external/webinar-compuware.git`
1. Run `docker-compose build` the docker containers should be built

1. `docker-compose up -d` 
