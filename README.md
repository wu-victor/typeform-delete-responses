# typeform-delete-responses

## Fork this repo
[Fork](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks) or copy this repo.

## Set up your Typeform API token
Create a [Typeform API token](https://www.typeform.com/developers/get-started/personal-access-token/) and save the value to your desktop.

In your new repo, add an [Actions secret](https://docs.github.com/en/actions/security-guides/using-secrets-in-github-actions) called `TYPEFORM_API_TOKEN` with the token you just created.

## Replace form id
In `delete-responses.yml`, replace the string value indicated by `TYPEFORM_FORM_ID` with the form id that you care about.
