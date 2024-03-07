# typeform-delete-responses

## Fork this repo
[Fork](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks) or copy this repo.

## Set up your Typeform API token
Create a [Typeform API token](https://www.typeform.com/developers/get-started/personal-access-token/) and save the value to your desktop.

In your new repo, add an [Actions secret](https://docs.github.com/en/actions/security-guides/using-secrets-in-github-actions) called `TYPEFORM_API_TOKEN` with the token you just created.

## Replace form id
In `delete-responses.yml`, replace the string value indicated by `TYPEFORM_FORM_ID` with the form id that you care about.

## Customize your workflow schedule
In `delete-responses.yml`, replace the cron schedule value to whenever you want your workflow to run. [crontab guru](https://crontab.guru/) is a helpful tool. The GitHub Actions [schedule](https://docs.github.com/en/actions/using-workflows/events-that-trigger-workflows#schedule) is not very reliable. So consider scheduling your job in frequently and at at weird hours and minutes to avoid high traffic load.

## Run the workflow manually
[Trigger the workflow manually](https://docs.github.com/en/actions/using-workflows/manually-running-a-workflow) by clicking `Run workflow`. You can do this immediately after making any changes to your repo to see the results.

## View workflow runs
View workflow runs by clicking the `Actions` tab in your repo.
