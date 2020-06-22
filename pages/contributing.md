---
title: Contributing
permalink: /contributing

layout: post
sidenav: contributing
subnav:
  - text: What would you like to do?
    href: '#what-would-you-like-to-do'
  - text: Issues
    href: '#issues'
  - text: Making Changes
    href: '#making-changes'
  - text: Small Changes
    href: '#small-changes'
  - text: Changes to Multiple Pages
    href: '#content-of-multiple-pages'
  - text: Big Changes
    href: '#big-changes'
  - text: Developing With Jekyll
    href: '#developing-with-jekyll'
  - text: Playbook Structure
    href: '#playbook-structure'
---
## What would you like to do?
- I want to [suggest a change](#issues).
- I want to [resolve an issue](#resolving-and-actioning-issues).
- I want to [make a change myself](#making-changes).

## Issues
### How to Create an Issue
Information on how to create an issue on GitHub can be found [here](https://help.github.com/en/github/managing-your-work-on-github/creating-an-issue). 

You can create an issue for this playbook [here](https://github.com/bcgov/CITZ-IMB-playbook/issues/new/).

### Guidelines for Creating Issues
To help our developers resolve your issue, we suggest the following:
- Include the URL of the page with the issue.
- If there is a typo, please include the selection of text that should be changed, along with the text to replace it.
- If the issue is regarding some visual aspect of the site, please include a screenshot highlighting what you would like changed.
- In general, please try to include as much information as possible.

### Resolving and Actioning Issues
When actioning an issue, consider [linking your pull request](https://help.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue). This not only allows for collaborators to see who is working on what issues, but it also makes it so that the issue is automatically closed when the pull request is merged.

Furthermore, take some time to consider what kind of change you are making. Is it a [small change](#small-changes), or a [big change](#big-changes)? This may determine how you resolve the issue.

## Making Changes
### What kind of change do you want to make?
- I want to make a [small change to a few words on one page](#small-changes).
- I want to make [changes to the content of multiple pages](#content-of-multiple-pages).
- I want to make [big changes to the look and/or structure of the site](#big-changes).

### Small Changes
If you really are just making small changes to a few words in one file, then it would be acceptable and easy to use the [GitHub file editor](https://help.github.com/en/github/managing-files-in-a-repository/editing-files-in-your-repository). This is not advisable for larger changes, or if you plan on making changes to multiple pages.

### Content of Multiple Pages
*Note: This section assumes some knowledge of Git.*

If you are making changes to the content of a few different pages then it would be best to do the following:
- Make a [fork](https://help.github.com/en/enterprise/2.13/user/articles/fork-a-repo#:~:text=A%20fork%20is%20a%20copy,point%20for%20your%20own%20idea.) of the [bcgov repo](https://github.com/bcgov/CITZ-IMB-playbook).
- Enable [GitHub Pages](https://help.github.com/en/github/working-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site) on the fork.
- [Clone](https://help.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository) your fork to your local machine.
- Ensure you are familiar with [Markdown](#a-note-on-markdown) syntax.
- Make any changes you are planning.
- Issue the following commands to push the changes to your forked repo:
~~~~ 
git add . 
git commit -m “Meaningful message about your changes”
git push origin master
~~~~
- Ensure everything looks good on your forked GitHub Pages site.
    - *Note: the way GitHub Pages compiles your website may differ than what you see during local development.*
- Make a [pull request](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/about-pull-requests).

### Big Changes
*Note: This section assumes some knowledge of Git and web development.*

If you are making big structural or visual changes to the playbook, we suggest that you get set up for local development on your computer. This increases efficiency by allowing you to preview the changes you are making in real time, and it reduces the risk of pushing errors to production.

To do this you must do the following:
- Make a [fork](https://help.github.com/en/enterprise/2.13/user/articles/fork-a-repo#:~:text=A%20fork%20is%20a%20copy,point%20for%20your%20own%20idea.) of the [bcgov repo](https://github.com/bcgov/CITZ-IMB-playbook).
- Enable [GitHub Pages](https://help.github.com/en/github/working-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site) on the fork.
- [Clone](https://help.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository) your fork to your local machine.
- Set up your workstation for [local jekyll development](#developing-with-jekyll).
- Familiarize yourself with the [structure of the playbook](#playbook-structure).
- Preview your changes with a local server.
- Issue the following commands to push the changes to your forked repo:
~~~~ 
git add . 
git commit -m “Meaningful message about your changes”
git push origin master
~~~~
- Ensure everything looks good on your forked GitHub Pages site.
    - *Note: the way GitHub Pages compiles your website may differ than what you see during local development.*
- Make a [pull request](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/about-pull-requests).

### A Note on Versioning
If the changes you are making to the site are quite large, consider creating a new version release. Please consult these resources before creating a new version:
- [Version releases with GitHub](https://help.github.com/en/github/administering-a-repository/managing-releases-in-a-repository)
- [Version tagging concepts](https://semver.org/) 

## Developing With Jekyll
### OS Recommendation
While Jekyll will work on Windows, it is not officially supported by the Jekyll team. If you only have access to Windows, please consider using [Windows Subsystem for Linux](https://docs.microsoft.com/en-us/windows/wsl/) for development.

### Getting Started
To get started developing with Jekyll, use this [guide](https://jekyllrb.com/docs/). The terminal will be very helpful if you are missing any packages, so be sure to read any error messages in detail.

### A Note on Markdown
The Markdown files that hold the playbook content live in the “plays” and “pages” folders. If you are unfamiliar with Markdown, [this](https://www.markdownguide.org/basic-syntax/) is a good place to get started.

## Playbook Structure
The playbook follows the general structure of a Jekyll site. If you wish to make large structural or navigational changes, the resources below should help you.

*Note: the following list is not exhaustive (as there is a wealth of Jekyll documentation available online), but it should be a good start.*
- [Directory Structure](https://jekyllrb.com/docs/structure/)
- [Configuring Site Navigation](https://jekyllrb.com/tutorials/navigation/)
- [Variables](https://jekyllrb.com/docs/variables/)
- [Includes](https://jekyllrb.com/docs/includes/)
- [Layouts](https://jekyllrb.com/docs/layouts/)

[Back to the Top](#)

