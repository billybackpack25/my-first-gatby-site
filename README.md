<p align="center">
  <a href="https://www.gatsbyjs.com/?utm_source=starter&utm_medium=readme&utm_campaign=minimal-starter">
    <img alt="Gatsby" src="https://www.gatsbyjs.com/Gatsby-Monogram.svg" width="60" />
  </a>
</p>
<h1 align="center">
  Cool Things
</h1>

## 🚀 Items

1. **Pages**

    In order to create a navigations link to a page,
    just create the page in src/pages with a default export.

    so src/pages/home.js

    ```jsx
    // Step 1: Import React
    import * as React from 'react'

    // Step 2: Define your component
    const IndexPage = () => {
      return (
        <main>
          <title>Home Page</title>
          <h1>Welcome to my Gatsby site!</h1>
          <p>Im making this by following the Gatsby Tutorial.</p>
        </main>
      )
    }

    // Step 3: Export your component
    export default IndexPage
    ```

2. **Linking to other pages**
    
    Linking to a page on your site, use `Link` 
    ```jsx
    import { Link } from 'gatsby'
    ```
    Linking to other pages `<a>`

3. **Styling**

    Styling a component can be done with CSS Modules, to prevent class naming collisions. End the filename in `src/components/my-component.module.css`

    ```jsx
    import { container } from './layout.module.css'

    const Layout = ({ pageTitle, children }) => {
    return (
        <main className={container}>
        </main>
      )
    }

    export default Layout
    ```

4. **Gatsby Plugins**
    [Plugins](https://www.gatsbyjs.com/plugins)

    In Gatsby terms, a plugin is a separate npm package that you install to add extra features to your site.

    - Install the plugin `npm install plugin-name`
    - Add the plugin to the `gatsby-config.js`
        ```javascript
        module.exports = {
          siteMetadata: {
            title: "My First Gatsby Site",
          },
          plugins: ["plugin-name"], // Here
        };
        ```
    - Some plugins may require extra `gatsby-config.js` use an object instead
      ```javascript
      plugins: [
        {
          resolve: "plugin-name",
          options: {
            // Check the plugin README for what options go in here
          }
        },
      ]
      ```
    - After you make updates to your `gatsby-config.js` file, you’ll need to restart your `gatsby develop` process for your changes to be picked up.
    - Use the plugin features in your site.


    5. **Performant Images**

    You can use the `gatsby-plugin-image` plugin to add responsive images to your site while maintaining high performance scores. `gatsby-plugin-image` exports a component called `StaticImage`, which you can use to load images from a remote URL or your local filesystem.

    - Install `npm install gatsby-plugin-image gatsby-plugin-sharp gatsby-source-filesystem`
    -         `npm install gatsby-plugin-image gatsby-plugin-sharp gatsby-source-filesystem gatsby-transformer-sharp`
    - Add to the `config` file
    ```javascript
        plugins: [
        "gatsby-plugin-gatsby-cloud",
        "gatsby-plugin-image",
        "gatsby-plugin-sharp"
      ],
    ```
    - Use the module in your page
    ```jsx
    import { StaticImage } from 'gatsby-plugin-image'

    <StaticImage
        alt="Clifford, a reddish-brown pitbull, posing on a couch and looking stoically at the camera"
        src="https://pbs.twimg.com/media/E1oMV3QVgAIr1NT?format=jpg&name=large"
      />

    <StaticImage
        alt="Clifford, a reddish-brown pitbull, posing on a couch and looking stoically at the camera"
        src="../images/clifford.jpg"
      />
    ```

  6. 





















































<p align="center">
  <a href="https://www.gatsbyjs.com/?utm_source=starter&utm_medium=readme&utm_campaign=minimal-starter">
    <img alt="Gatsby" src="https://www.gatsbyjs.com/Gatsby-Monogram.svg" width="60" />
  </a>
</p>
<h1 align="center">
  Gatsby minimal starter
</h1>

## 🚀 Quick start

1.  **Create a Gatsby site.**

    Use the Gatsby CLI to create a new site, specifying the minimal starter.

    ```shell
    # create a new Gatsby site using the minimal starter
    npm init gatsby
    ```

2.  **Start developing.**

    Navigate into your new site’s directory and start it up.

    ```shell
    cd my-gatsby-site/
    npm run develop
    ```

3.  **Open the code and start customizing!**

    Your site is now running at http://localhost:8000!

    Edit `src/pages/index.js` to see your site update in real-time!

4.  **Learn more**

    - [Documentation](https://www.gatsbyjs.com/docs/?utm_source=starter&utm_medium=readme&utm_campaign=minimal-starter)

    - [Tutorials](https://www.gatsbyjs.com/tutorial/?utm_source=starter&utm_medium=readme&utm_campaign=minimal-starter)

    - [Guides](https://www.gatsbyjs.com/tutorial/?utm_source=starter&utm_medium=readme&utm_campaign=minimal-starter)

    - [API Reference](https://www.gatsbyjs.com/docs/api-reference/?utm_source=starter&utm_medium=readme&utm_campaign=minimal-starter)

    - [Plugin Library](https://www.gatsbyjs.com/plugins?utm_source=starter&utm_medium=readme&utm_campaign=minimal-starter)

    - [Cheat Sheet](https://www.gatsbyjs.com/docs/cheat-sheet/?utm_source=starter&utm_medium=readme&utm_campaign=minimal-starter)

## 🚀 Quick start (Gatsby Cloud)

Deploy this starter with one click on [Gatsby Cloud](https://www.gatsbyjs.com/cloud/):

[<img src="https://www.gatsbyjs.com/deploynow.svg" alt="Deploy to Gatsby Cloud">](https://www.gatsbyjs.com/dashboard/deploynow?url=https://github.com/gatsbyjs/gatsby-starter-minimal)
