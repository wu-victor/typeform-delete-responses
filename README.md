# typeform-delete-responses

> [!WARNING]  
> This repo is not endorsed and not supported by Typeform the company. If you use this code, it may have unintended consequences, including deleting Typeform data that you did not want deleted, and that is **not recoverable**. It has not been thoroughly tested. There are likely bugs and edge cases. Use at your own risk.

## Delete Typeform responses on a schedule with GitHub Actions
This repo deletes responses in a specified Typeform using the [Typeform Responses API](https://www.typeform.com/developers/responses/). It runs inside [GitHub Actions](https://docs.github.com/en/actions), which is a  serverless environment that allows for scheduled jobs. GitHub Actions is a free offering already integrated within any GitHub repo. So you can fork/copy this repo, make changes, and run the code all within GitHub.

## Fork/copy this repo
[Fork](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks) or copy this repo.

## Set up your Typeform API token
Create a [Typeform API token](https://www.typeform.com/developers/get-started/personal-access-token/) and save the value to your desktop.

In your new repo, add an [Actions secret](https://docs.github.com/en/actions/security-guides/using-secrets-in-github-actions) called `TYPEFORM_API_TOKEN` with the token you just created.

## Replace form id
In `delete-responses.yml`, replace the string value indicated by `TYPEFORM_FORM_ID` with the form id that you care about.

## Customize your workflow schedule
In `delete-responses.yml`, replace the cron schedule value to whenever you want your workflow to run. [crontab guru](https://crontab.guru/) is a helpful tool. The GitHub Actions [schedule](https://docs.github.com/en/actions/using-workflows/events-that-trigger-workflows#schedule) is not very reliable. So consider scheduling your job infrequently and at at weird hours and minutes to avoid high traffic load.

## Run the workflow manually
[Trigger the workflow manually](https://docs.github.com/en/actions/using-workflows/manually-running-a-workflow) by clicking `Run workflow`. You can do this immediately after making any changes to your repo to see the results.

## View workflow runs
View workflow runs by clicking the `Actions` tab in your repo.
