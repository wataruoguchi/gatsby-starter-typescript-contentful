<p align="center">
  <a href="https://www.gatsbyjs.org">
    <img alt="Gatsby" src="https://www.gatsbyjs.org/monogram.svg" width="60" />
  </a>
</p>
<h1 align="center">
  Gatsby TypeScript Contentful starter
</h1>

This starter is TypeScript version of the [Gatsby's default starter](https://github.com/gatsbyjs/gatsby-starter-default) with Contentful Integration. I am trying it as simple as possible.

## 🚀 Quick start

1.  **Create a Gatsby site.**

    Use the Gatsby CLI to create a new site, specifying the default starter.

    ```shell
    # install the Gatsby CLI
    npm install -g gatsby-cli
    # create a new Gatsby site using the default starter
    gatsby new my-default-starter https://github.com/wataruoguchi/gatsby-starter-typescript-contentful
    ```

1)  **Set up Contentful**

    If you're using Contentful for the first time, you can follow steps below. That way, you can display contents without changing `src/pages/blogPosts.tsx`.

    1. Sign up [Contentful](https://www.contentful.com/sign-up/)
    1. Create a Space.
    1. Create a Content model(content type).
       - The content type name should be `Blog Post` (more specifically, the content type id should be `blogPost`).
       - It should have following fields:
         - title (Short text)
         - body (Rich text)
    1. Create a content.

1)  **Start developing.**

    Navigate into your new site’s directory, configure and start it up.

    ```shell
    cd my-default-starter/
    cp .env{.default,}
    ```

    Then update `.env` file. You can get Space ID and access token in Contentful.

    Start it up:

    ```shell
    gatsby develop
    ```

1)  **Open the source code and start editing!**

    Your site is now running at `http://localhost:8000`!

    _Note: You'll also see a second link: _`http://localhost:8000/___graphql`_. This is a tool you can use to experiment with querying your data. Learn more about using this tool in the [Gatsby tutorial](https://www.gatsbyjs.org/tutorial/part-five/#introducing-graphiql)._

    Open the `my-default-starter` directory in your code editor of choice and edit `src/pages/index.js`. Save your changes and the browser will update in real time!

## 🧐 What's inside?

A quick look at the top-level files and directories you'll see in a Gatsby project.

    .
    ├── node_modules
    ├── src
    ├── .env.default
    ├── .gitignore
    ├── .prettierrc
    ├── gatsby-browser.js
    ├── gatsby-config.js
    ├── gatsby-node.js
    ├── gatsby-ssr.js
    ├── LICENSE
    ├── package-lock.json
    ├── package.json
    └── README.md

1.  **`/node_modules`**: This directory contains all of the modules of code that your project depends on (npm packages) are automatically installed.

2.  **`/src`**: This directory will contain all of the code related to what you will see on the front-end of your site (what you see in the browser) such as your site header or a page template. `src` is a convention for “source code”.

3.  **`/src/pages/blogPosts.tsx` and `/src/components/contentfulRichText.tsx`**: These are the additional files that the default starter does not have. The component parses Contentful rich text contents, and the page displays contents from Contentful.

4.  **`.gitignore`**: This file tells git which files it should not track / not maintain a version history for.

5.  **`gatsby-browser.js`**: This file is where Gatsby expects to find any usage of the [Gatsby browser APIs](https://www.gatsbyjs.org/docs/browser-apis/) (if any). These allow customization/extension of default Gatsby settings affecting the browser.

6.  **`gatsby-config.js`**: This is the main configuration file for a Gatsby site. This is where you can specify information about your site (metadata) like the site title and description, which Gatsby plugins you’d like to include, etc. (Check out the [config docs](https://www.gatsbyjs.org/docs/gatsby-config/) for more detail).

7.  **`gatsby-node.js`**: This file is where Gatsby expects to find any usage of the [Gatsby Node APIs](https://www.gatsbyjs.org/docs/node-apis/) (if any). These allow customization/extension of default Gatsby settings affecting pieces of the site build process.

8.  **`gatsby-ssr.js`**: This file is where Gatsby expects to find any usage of the [Gatsby server-side rendering APIs](https://www.gatsbyjs.org/docs/ssr-apis/) (if any). These allow customization of default Gatsby settings affecting server-side rendering.

9.  **`LICENSE`**: Gatsby is licensed under the MIT license.

10. **`yarn.lock`** (See `package.json` below, first). This is an automatically generated file based on the exact versions of your npm dependencies that were installed for your project. **(You won’t change this file directly).**

11. **`package.json`**: A manifest file for Node.js projects, which includes things like metadata (the project’s name, author, etc). This manifest is how npm knows which packages to install for your project.

12. **`README.md`**: A text file containing useful reference information about your project.

13. **`.env.default`**: A template file for `.env`. You are not supposed to update this file but `.env` file.

14. **`.eslintrc.js`**: ESLint config file.

15. **`.huskyrc.js`**: Husky config file.

16. **`.prettierignore`**: This file tells prettier which file it should ignore.

17. **`.prettierrc.js`**: Prettier config file.

18. **`lint-staged.config.js`**: lint-staged config file.

19. **`stylelint.config.js`**: StyleLint config file.

20. **`tsconfig.json`**: TypeScript config file.

## 🎓 Learning Gatsby

Looking for more guidance? Full documentation for Gatsby lives [on the website](https://www.gatsbyjs.org/). Here are some places to start:

- **For most developers, we recommend starting with our [in-depth tutorial for creating a site with Gatsby](https://www.gatsbyjs.org/tutorial/).** It starts with zero assumptions about your level of ability and walks through every step of the process.

- **To dive straight into code samples, head [to our documentation](https://www.gatsbyjs.org/docs/).** In particular, check out the _Guides_, _API Reference_, and _Advanced Tutorials_ sections in the sidebar.

## 💫 Deploy

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/gatsbyjs/gatsby-starter-default)
