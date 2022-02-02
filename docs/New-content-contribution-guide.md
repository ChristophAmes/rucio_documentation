---
id: new-content-contribution-guide
title: New Content Contribution Guide
sidebar_label: New Content Contribution Guide
---

There are two types of documentation hosted on Rucio as detailed
in the [types of pages](types-of-pages.md) section. Should you wish to
add content to any of them, kindly follow the guidelines below
per the section.

## API Documentation

The source for this section lives in the
[`rucio/rucio`](https://github.com/rucio/rucio) GitHub repository. Below are the
two sub-categories that we maintain documentation for:

- [__Rest API__](https://github.com/rucio/rucio/tree/master/lib/rucio/web/rest/flaskapi/v1)

- [__Client API__](https://github.com/rucio/rucio/tree/master/lib/rucio/client)

Since the documentation is directly derived from the source by Sphinx, ensure
you're incorporating the relevant information into the respective `.py` files.
Existing `.py` files in the directories should give you an idea of how this is
done across the project.  Once the changes have been approved & pushed into the
main branch, you will need to submit a Pull Request to the **sphinx** branch of
the [`rucio/documentation`](https://github.com/rucio/documentation) repository
so that the changes can be reflected on the website.

## Markdown documentation

The source for this section lives in the `docs` folder within the **master**
branch of the [`rucio/documentation`](https://github.com/rucio/documentation)
GitHub repository. Any content that needs to be added should be written in
Markdown and added to this folder. Should you wish to add it to the sidebar for
ease of navigation, you will also need to modify `sidebars.json`.  Once the
changes are approved, GitHub actions will trigger the build process for merging
your changes with the master branch.
