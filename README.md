# pixincreate.dev

[![Staging or PR preview](https://github.com/pixincreate/pixincreate.dev/actions/workflows/pr-preview.yml/badge.svg)](https://github.com/pixincreate/pixincreate.dev/actions/workflows/pr-preview.yml) [![Production](https://github.com/pixincreate/pixincreate.dev/actions/workflows/CI.yml/badge.svg)](https://github.com/pixincreate/pixincreate.dev/actions/workflows/CI.yml)

Welcome to my portfolio website repository! This site is built using the Hugo static site generator and uses the [Hello-Friend-NG](https://github.com/rhazdon/hugo-theme-hello-friend-ng) theme to showcase my work, projects, and achievements. It's deployed through Cloudflare using GitHub CI/CD for a seamless and efficient workflow.

## Table of Contents

- [Introduction](#introduction)
- [How to Build](#how-to-build)
- [License](#license)
- [Disclaimer](#disclaimer)

## Introduction

This repo is the home of **_pixincreate.dev_** and the source is available within this repo. **_pixincreate.dev_** is a "to-be-static" website and is stands as the portfolio website of _Pa1NarK_. **_pixincreate.dev_** is an entry point where you get to see all of my work and experience.

## How to Build

I discourage you from using this repo as your base given that you will have to go through all the changes Pa1Nark has done.

To start with, install [`HUGO`](https://gohugo.io/installation/) and [Git](https://git-scm.com/download) as a pre-requisite.

1. Create a HUGO project:

    ```sh
    hugo new site <your-website-name>
    cd  <your-website-name>
    ```

2. Initialize you Git repository:

    ```sh
    git init
    git submodule add https://github.com/rhazdon/hugo-theme-hello-friend-ng.git themes/hello-friend-ng
    # Optionally,  you can try running this once as well:
    git submodue update --recursive
    ```

3. Add theme to `hugo.toml`

    ```sh
    echo "theme = 'hello-friend-ng'" >> hugo.toml
    ```

4. Starti server for testing:

    ```sh
    # To run in 'development' environment.
    # This will start a development server. You can preview your site by opening a web browser and navigating to `http://localhost:1313`.
    hugo server
    # To run locall in 'staging environment'
    hugo server --environment "staging"
    ```

5. **Customize Your Content:**
    Modify the content in the `content/` directory to reflect your portfolio. Hugo is highly customizable, and you can edit configuration files in the `hugo.toml` file to adjust site settings.

    ```sh
    hugo new <file-name>.md
    ```

    This should create a content file for you to work with.
    You can refer to HUGO's [Getting-Started](https://gohugo.io/getting-started) to learn to work with the file-system
    Prefereably, it is receommended that you go through [Hello-Friend-NG](https://github.com/rhazdon/hugo-theme-hello-friend-ng) theme's GitHub repo to learn about the custom commands that are specific tothe theme and the options that it provides

6. **Build the Site:**

   When you are ready to deploy your site, run:

   ```bash
   hugo --gc --minify
   ```

   This should run in `production` environment

7. **Deploy with GitHub CI:**

    This repository is set up with GitHub CI/CD to automatically deploy changes to Cloudflare-hosted site. Make sure to configure your Cloudflare settings and GitHub Actions workflow as needed.

    7.1 **Buy a Domain**

        You can buy domain at `namecheap` or `cloudflare registrar`

    7.2 **Set up cloudflare**

        - Set-up your cloudflare account, and create a cloudflare page  
        - Add the custom domain you bought in the project's custom domain section

## License

This project is licensed under the [CC0 1.0 Universal (CC0 1.0) License](LICENSE). You are free to use and modify this project for your own purposes. For more details, see the [LICENSE](LICENSE) file.

## Disclaimer

YOU SHOULD NOT MISUSE ANY INFORMATION, CONTENT, OR SERVICES PROVIDED ON THIS WEBSITE. IF YOU CHOOSE TO MISUSE, IT IS YOUR RESPONSIBILITY, AND YOU ACCEPT THE CONSEQUENCES.
I DISCLAIM ANY LIABILITY FOR ANY DAMAGES, LOSSES, OR CONSEQUENCES RESULTING FROM YOUR ACTIONS, WHETHER INTENTIONAL OR UNINTENTIONAL, BASED ON THE INFORMATION, CONTENT, OR SERVICES OFFERED ON THIS WEBSITE.
THIS DISCLAIMER SERVES AS A CLEAR NOTICE THAT YOU ARE SOLELY ACCOUNTABLE FOR YOUR BEHAVIOR AND INTERACTIONS ON THIS WEBSITE. I WILL NOT BE HELD RESPONSIBLE FOR ANY MISUSE, HARASSMENT, MALICIOUS INTENT, OR OTHER ACTIVITIES THAT MAY RESULT FROM YOUR ENGAGEMENT WITH THIS SITE.
BY ACCESSING AND USING THIS WEBSITE, YOU ACKNOWLEDGE AND AGREE TO THIS DISCLAIMER. IF YOU DISAGREE WITH ANY PART OF THIS DISCLAIMER, PLEASE REFRAIN FROM USING THIS WEBSITE.
THIS DISCLAIMER APPLIES TO ALL USERS, VISITORS, AND INTERACTIONS ON THIS WEBSITE.
