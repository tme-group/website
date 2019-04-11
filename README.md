# KAMP

## Getting Started

To get started with KAMP, make sure you have Node and Yarn installed on your machine.

You can install Yarn through the Homebrew package manager. This will also install Node.js if it is not already installed.

```
brew install yarn
```

After installing Yarn, install the Gatsby-CLI.

```
yarn global add gatsby-cli
```

Clone the project

```
git clone git@github.com:kamp-group/website.git
```

In the project root, install all dependencies

```
yarn install
```

Once all dependencies are install, you can start the development server

```
yarn dev
```

The site will be available at localhost:3000

## Creating a post

You can create a new post by creating a folder within `/src/pages/article/`. The folder name will be the slug url of the post.

Create an `index.md` file in the folder to start.

Posts need to have a layout type. Currently, the available post types are `text-post`, `image-post`, and `video-post`.

## Changing the style or layout of a post

The layout for each post type is in the `/src/tempaltes/` folder. (`blog-post` corresponds to `text-post`)

The styles for each post type are in their own .scss file in `/src/styles`. To style a specific post type, add classes (with `className` _because javascript_) to the template, then use the class in the .scss file.

## Publishing your changes

All code merged to master will publish on the live site, unless there is a build error. If there is a build error, the older, working version of the site will stay live.
