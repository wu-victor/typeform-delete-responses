# typeform-delete-responses

## Fork this repo
[Fork](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks) or copy this repo.

## Set up your Typeform API token
Create a [Typeform API token](https://www.typeform.com/developers/get-started/personal-access-token/). Add that token to your new repo as an Actions secret called `TYPEFORM_API_TOKEN`.

In your new repo, add an [Actions secret](https://docs.github.com/en/actions/security-guides/using-secrets-in-github-actions) called `TYPEFORM_API_TOKEN`.

## Replace form id
In `delete-responses.yml`, replace the string value indicated by `TYPEFORM_FORM_ID` with the form id that you care about.
