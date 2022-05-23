# Commons campaigns

The [`campaigns.json`](https://github.com/commons-app/campaigns/blob/master/campaigns.json) file contains information (title, description, dates, link) about Commons campaigns such as Wiki Loves Monuments.

Campaigns will be advertised in the [Commons Android app](https://github.com/commons-app/apps-android-commons/) using this information.

All campaigns found [here](https://commons.wikimedia.org/wiki/Category:Photography_competitions) are eligible.

## Adding or modifying a campaign

If a campaign is not documented yet, or to modify the dates or URL, please:

1. Go to the [campaign editor](https://commons-app.github.io/campaigns-editor/)
2. Click `Add` and enter the details for the campaign
3. Scroll down to the result, click `Copy to clipboard` and then `Edit on GitHub`
4. Delete the existing content, and paste in the updated campaigns file
5. In the pull request description, provide a source for the information, for instance a link to an announcement or wiki discussion
6. We will review your contribution and merge it
7. After your PR is merged, check the app displays the campaign correctly and report any problems

Thanks!

## Using the campaigns data

Make a GET request to the GitHub API to fetch the JSON file. For example:

```
curl -X GET https://raw.githubusercontent.com/commons-app/campaigns/master/campaigns.json
```