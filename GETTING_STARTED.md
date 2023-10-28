# Getting Started

This is a guide to help you get started with the Braingeneers Python Research Template. This template is designed to help you get started with your own research project. It is designed to be flexible and modular, so that you can easily add new features and functionality as you need it.

## Using Codespaces

The easiest way to get started is to use GitHub Codespaces. This will allow you to run the code in the cloud, without having to install anything on your computer. To get started, click the green "Code" button at the top of this page, and select "Open with Codespaces". This will open a new Codespace for you, and you can start working right away.

### Open with Codespaces

Inside of the `README.md` file, you will find a link to open the project in Codespaces. Clicking this link will open a new Codespace for you, and you can start working right away. To update the repo name connected to the "Open with Codespaces" button, you will need to update the `README.md` code.

```md
[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/braingeneers/<project_name>?quickstart=1)
```

For example:

```md
[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/braingeneers/python-research-template?quickstart=1)
```

Review the [Codespaces documentation](https://docs.github.com/en/github/developing-online-with-codespaces/creating-a-codespace#creating-a-codespace-using-a-template-repository) for more information.

### Customize Codespace

To change the name of your Codespace, click the "Customize" button in the bottom left corner of the screen.

## Running Locally

If you want to run the code locally, you will need to install Python 3.7 or higher. You can download Python from [python.org](https://www.python.org/downloads/). You will also need to install [Git](https://git-scm.com/downloads) if you don't already have it.

## Citations with Zenodo

This guide will help you set up Zenodo DOI badges and enable the integration between your GitHub repository and Zenodo to ensure proper citation of your work.

### 1. Setup Zenodo DOI Badge Before the First Release

Before you submit your first release on Zenodo, it's essential to set up the Zenodo DOI badge in your project's documentation or README.

#### Add the Zenodo DOI Badge

1. Obtain your Zenodo DOI badge. You will receive this DOI after your first release on Zenodo.

   ![Zenodo DOI Badge](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.1234567-blue.svg)

2. Locate your GitHub repository ID by accessing the GitHub API. Replace `{user}` with your GitHub username and `{repo}` with your repository name in the following URL:

   ```bash
   https://api.github.com/repos/{user}/{repo}
   ```

3. Once you have the GitHub repository ID, add the Zenodo DOI badge to your project's `README.md` or `README.rst` file.

#### For `README.md`

In your `README.md` file, add the following Markdown code, replacing `{github_id}` with your GitHub repository ID:

```markdown
[![DOI](https://zenodo.org/badge/{github_id}.svg)](https://zenodo.org/badge/latestdoi/{github_id})
```

#### For `README.rst`

If you're using reStructuredText for your documentation, add the following code, replacing `{github_id}` with your GitHub repository ID:

```rst
|DOI|

.. |DOI| image:: https://zenodo.org/badge/{github_id}.svg
        :target: https://zenodo.org/badge/latestdoi/{github_id}
```

### 2. Submit Your First Release

After adding the Zenodo DOI badge, you are ready to submit your first release. Keep in mind the following notes:

__Notes:__
- The DOI badge will not be issued until you make your first release, but it will be included in your release.
- To set up Zenodo webhooks with GitHub for automated releases, you can refer to the [GitHub documentation](https://guides.github.com/activities/citable-code/).

By following these steps, you ensure that your project is appropriately cited and can be easily referenced by others in the academic and research communities.
