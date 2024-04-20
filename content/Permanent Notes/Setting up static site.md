---
title: Setting up static site
draft: false
tags:
---
---
I've recently set up Quartz for Obsidian nodes and found the process to be fairly straightforward. Here's a breakdown of the steps I took and some insights that might help anyone looking to do the same.

### Basic Installation

- Followed the basic setup instructions provided in the [Quartz documentation.](https://quartz.jzhao.xyz/)
- The key aspect to keep in mind during setup is how the linkages happen. A recommended implementation for Obsidian should be selected.

### Pushing Code to Remote Server on GitHub

1. **Remove the Upstream Branch**: The first step involves removing the existing upstream branch using the command `git rm remote`. This clears the way for you to add your own.
2. **Add Your Own Upstream Repository**: After removing the default upstream branch, you can add your own repository as the new upstream. This step is crucial for keeping your blog up to date.

### Publishing Your Site

After setting up the Quartz and pushing the code to GitHub, the next step is to publish your site. There are several platforms available for this, but I chose Cloudflare for its straightforward process.

- **Using Cloudflare**:
  - Log in to Cloudflare
  - In account Home, select **Workers & Pages** > **Create application** > **Pages** > **Connect to Git**.
  - It prompts you to connect to GitHub. Once connected, select the repository you wish to publish.
  - Cloudflare takes care of most of the setup after this point. There's just a minor configuration needed, but it's quite straightforward.

### Conclusion

The entire process, from setting up Quartz for Obsidian nodes to publishing the site on Cloudflare, was simpler than expected. The key is to follow the documentation closely and make sure the GitHub repository is correctly linked for updates. Cloudflare proved to be an efficient choice for hosting, with an easy setup that integrates seamlessly with GitHub.