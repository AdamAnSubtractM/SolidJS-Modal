<p align="center">
  <a href="https://adamknee.dev">
    <img alt="Adam Knee's Logo" src="https://res.cloudinary.com/adamansubtractm/image/upload/r_20/v1662130192/github/logo-w-banner-blue_raujqx.svg" width="2000" />
  </a>
</p>

# Modal in SolidJS with Typescript

This repo contains the completed code for the [@AdamAnSubtractM](https://youtu.be/HSoRtowmOEY) "How to make a Modal in SolidJS with Typescript" tutorial.

## Prerequisites

- Must have node version `18.7.0`. I highly recommend you use a node version manager if you don't already. See the section "Using and Installing a Node Version Manager"
- [Recommended] - `pnpm` installed to manage package dependencies. You can ofcourse use `npm` which will come with your node version or `yarn` if you'd like. I prefer `pnpm` simply because of the way it handles dependencies and in addition to that, it tends to log less garbage than `npm` does. I am also aware that `pnpm` has its own node manager but I'm much more familiar with others, so I will continue using those for these tutorials. Use what you're comfortable/familiar with. See the section "Using and Installing `pnpm`"

## Using and Installing a Node Version Manager

First things first, if you're not already using a node version manager, you're doing yourself a serious disservice. A node manager will change your life! A node manager allows you to easily and quickly switch between versions of node. This is sometimes important depending on the project you're working on.

### Windows Users

- I am not a Windows user and the only node version manager I'm familiar with for Windows is "NVM for Windows". You can find [installation instructions here](https://github.com/coreybutler/nvm-windows). Once installed, you can use `nvm` the same way Mac users can. To install and use a version of node using nvm, do the following (you may need to complete these steps as an admin user):

```bash
# Step 1 - nvm install <verison>
nvm install 18.7.0
# Step 2 - nvm use <version>
nvm use 18.7.0
```

- Alternatively, you may be able to use the node version manager provided with `pnpm`. Unfortunately, I'm not super familiar with that process yet but feel free to read up on that if that's easiest for you

### Mac Users

You have a few options for a node manager as a Mac user. `nvm` and `n`. Personally, I prefer the latter option, `n`. Bullet point number 1 will cover the `nvm` installation and bullet point number 2 [my preference] will cover the `n` installation.

- [Choice 1] - To install `nvm`, you can do it a few ways:

  - [Option 1] - Using `curl`:

    ```bash
    curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash
    ```

  - [Option 2] - Using `wget`:

    ```bash
    wget -qO- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash
    ```

  - [Option 3] - Using `homebrew`:

    ```bash
    brew install nvm
    ```

  - To use `nvm`:

    ```bash
    # Step 1 - sudo nvm install <verison>
    sudo nvm install 18.7.0
    # Step 2 - sudo nvm use <version>
    sudo nvm use 18.7.0
    ```

- [Choice 2] - My preference - To install `n`, you can do it a few ways:

  - [Option 1] - Using `npm` (this _only_ works if you already have a version of node installed):

    ```bash
    npm i -g n
    ```

  - [Option 2] - Using `hombrew`:

    ```bash
    brew install n
    ```

  - To use `n`:

    ```bash
    # Step 1 - sudo n <version> OR sudo n latest
    sudo n 18.7.0 # currently the latest version at the time this doc was written
    # Step 2 - if you need to switch versions: sudo n
    sudo n # use your arrow keys to select the version
    ```

## Using and Installing `pnpm`

### Windows Users

```bash
iwr https://get.pnpm.io/install.ps1 -useb | iex
```

### Mac Users

- [Option 1] - Using `curl`:

  ```bash
  curl -fsSL https://get.pnpm.io/install.sh | sh -
  ```

- [Option 2] - Using `wget`:

  ```bash
  wget -qO- https://get.pnpm.io/install.sh | sh -
  ```

- [Option 3] - Using `hombrew`:

  ```bash
  brew install pnpm
  ```

## SolidJS/Project Info

### Learn more on the [Solid Website](https://solidjs.com) and come chat with us on our [Discord](https://discord.com/invite/solidjs)

## Available Scripts

In the project directory, you can run:

### `pnpm dev` or `pnpm start`

Runs the app in the development mode.<br>
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br>

### `pnpm run build`

Builds the app for production to the `dist` folder.<br>
It correctly bundles Solid in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br>
Your app is ready to be deployed!

## Deployment

You can deploy the `dist` folder to any static host provider (netlify, surge, now, etc.)
