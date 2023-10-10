# invite_automator
Invite students to Self-Paced Curriculum

A django web app hosted somewhere that self-paced students use. It is an automation hook that was written by Mike Lee several years ago on a small Django server. When people sign up for the self paced course and you provide a github handle it automates the invitation process to the repo.
This form on the CP website goes to the invite automator: https://www.codeplatoon.org/self-paced/
This sends an e-mail to Rod which he has a forwarding rule to Zapier, not sure if you've checked that out yet or not, that then pings this server on heroku which then pings the Github AP

## env vars

These env / config vars are needed for the app to run. Reach out to get real values for them. 


```
DATABASE_URL  postgres://<POSTGRES_URL>
GH_T          <GITHUB_AUTH_TOKEN_HERE>
GH_U          <GITHUB_USERNAME_HERE>
HOST          https://<URL_OF_SERVER_HOSTING_THIS_APP_HERE>
SECRET_KEY    <SECRET_KEY_HERE>
```
