# GitHub Pages Redirect to /dev/null

This repository redirects visitors from [github](https://abusofianid.github.io) to my profile on [/dev/null](https://dev-null.sh/@abusofianid)

## How It Works

> To use this setup for a GitHub Pages user site, the repository name must follow this format: `<username>.github.io` 

The redirect is implemented using an HTML meta refresh tag in the root "index.html" file.

```html
<!doctype html>
<meta http-equiv="refresh" content="0;url=https://dev-null.sh/@abusofianid">
```

When a visitor opens the GitHub Pages URL, the browser automatically redirects them to the configured destination.

## GitHub Pages Setup

Follow these steps to configure GitHub Pages for this repository:

1. Open this repository on GitHub.
2. Navigate to Settings.
3. Select Pages under the Code and automation section.
4. Under Build and deployment, set Source to Deploy from a branch.
5. Select "main" as the publishing branch.
6. Select "/(root)" as the folder.
7. Click Save if the button is available.

GitHub Pages will publish the site from the root directory of the "main" branch. The root "index.html" file must exist in the selected publishing source.

After deployment, open "abusofianid.github.io" to verify the redirect.

## How to Change the Redirect URL

Follow these steps to update the destination:

1. Open this repository on GitHub.
2. Open the "index.html" file.
3. Click the edit button.
4. Replace the URL in the "content" attribute with your desired destination.
5. Commit the changes to the "main" branch.

For example, to redirect visitors to a different profile, update the HTML as follows:

```html
<!doctype html>
<meta http-equiv="refresh" content="0;url=https://dev-null.sh/your-profile">
```

Replace "https://dev-null/your-profile" with your /dev/null URL.
