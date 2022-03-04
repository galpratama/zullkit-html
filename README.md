# Tailwind CSS as a PostCSS Plugin

A starter template for very simple projects (no frameworks) with Tailwind CSS setup as a PostCSS plugin. You only need to install NPM.

Follow the Getting Started guide and build websites with Tailwind CSS. Also, follow the steps to Optimize for Production to end up with a very tiny final CSS bundle.

## Getting Started

1.  Clone the repository. Alternately you can download the zip file and unzip it.

2.  You will now have the cloned project folder. Open the project in
    Visual Studio Code editor (recommended code editor for Tailwind CSS
    Projects)

3.  Open new terminal within Visual Studio Code

4.  Download and install Yarn

5.  Install dependencies

        yarn

6.  Build using Tailwind CSS

        yarn build

7.  Open the `public > index.html` file in your browser and you should see a heading styled with a gradient. If you don't see a gradient on the text, something went wrong.

## How to use

-   Go to `public > index.html` Remove the `<h1>` element and start adding your own HTML.
-   If you need to add more HTML pages, add them in the `public` folder.
-   To extract classes and use the `@apply` directive, edit the custom CSS file in `src > styles.css`. Add any amount of custom CSS within this file. Refer [https://tailwindcss.com/docs/installation#using-a-custom-css-file](https://tailwindcss.com/docs/installation#using-a-custom-css-file)

Watch HTML files for changes and build automatically everytime using

    yarn watch

NOTE: Do NOT edit the file `public > dist > styles.css` directly - This is the distribution stylesheet. The CSS here is generated from `src > styles.css` using Tailwind when you build.

## Optimize for production

Before pushing your code (the `public` folder) for production, run the below command to reduce the size of `styles.css` within the public folder

     yarn prod

NOTE: If you are using Windows and face an error `NODE ENV not recognised`, run the below command

     yarn add win-node-env
