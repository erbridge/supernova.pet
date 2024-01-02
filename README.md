# supernova.pet

## Making changes

### Update your local repository

Pull the latest changes to this repository from GitHub:

1. Open GitHub Desktop
2. Switch the active branch to `main`
3. Click "Fetch origin" (this might not be necessary if "Pull origin" is already
   showing)
4. Click "Pull origin" if there are any updates

### Create a new branch

In GitHub Desktop, create a new branch in this repository for your changes.

### Start Hugo

Open a terminal to the root of this respository and run:

```sh
hugo server -D
```

### Make your changes

Make whatever changes you need in your editor (eg Visual Studio Code). You
should see your changes at http://localhost:1313/.

### Commit and push your changes

In GitHub Desktop:

1. Select the changes you want to keep
2. Write a short message explaining what you did
3. Press "commit"
4. Publish the branch to GitHub

### Create a pull request

In GitHub Desktop press "Preview pull request" and follow the steps until you
have created a pull request on the GitHub website.

### Preview and review your changes

After a few minutes, Render will comment on your pull request on the GitHub
website with instructions on how to preview your changes before making them
live.

If you need to make changes, you can commit to same branch, publish the new
changes, and Render will rebuild the page.

### Merge the pull request

If everything looks good in the preview, merge the pull request on the GitHub
website.

### Check your changes

After a few minutes, your changes should be merged and live.

## Setting up from scratch

### Clone this repository

Clone this repository to your local environment using your preferred method.

### Install Hugo

You'll need to install the correct version of [Hugo](https://gohugo.io/) for
this project.

1. Find the specific version of Hugo needed in [`.hugo-version`](.hugo-version).
2. Download that version for your operating system (macOS is also known as
   `darwin`) from
   [Hugo's releases on GitHub](https://github.com/gohugoio/hugo/releases). Note
   the `extended` prefix.
3. Unpack the downloaded `.tar.gz` file. On macOS, opening it in Finder will do
   this for you.
4. Install Hugo by copying the unpacked `hugo` executable to somewhere on your
   `PATH`, eg `/usr/local/bin`.
5. Run `hugo version` in your terminal to test things are working.
   [On macOS, you might need to bypass Gatekeeper](https://support.apple.com/en-us/HT202491).

Alternatively, you can use [`hugoenv`](https://github.com/erbridge/hugoenv) to
manage your Hugo installation for you.

### Connect to Airtable (optional)

If you want to be able to see data in the calendars, you'll need to set the
Airtable environment variables specified in [`.envrc.example`](.envrc.example).
If `HUGO_AIRTABLE_BASE_ID` is not set, the calendars will render without any
event data.
