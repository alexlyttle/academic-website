# academic-website

Guide to building a personal academic website.

## What Makes a Personal Academic Website?

Here is some suggested minimum content

- Your name and current affiliation
- A short biography
- Selected publications
- Selected projects/code
- Contact details

Here are some other things you could include,

- Links to social media 
- A link to your CV
- Teaching courses and links to material
- A blog
- Press releases
- List of people in your research group

## Creating a Static HTML Website

1. Follow instructions at [pages.github.com](https://pages.github.com/) to create the base repository for your website. It should be called `<username>.github.io`.

2. To create a static HTML5 website, you can start from scratch or download a template from e.g. [HTML5 UP](https://html5up.net).

3. Clone your repository,
   
   ```bash
   git clone https://github.com/<username>/<username>.github.io
   ```

4. Copy the contents of an HTML5 template into your repository

   - E.g. this site was made with the [Strata](https://html5up.net/strata) template

5. Open `index.html` locally in a text editor and in a browser

6. Make changes to `index.html` and refresh your browser. See what effect the changes have.

## Publishing a New Repository with GitHub Pages

If you have already created `<username>.github.io` and want to deploy a new repository to GitHub pages:

1. Create the repository called `<reponame>`

2. Go to the repository "Settings" tab at `https://github.com/<username>/<reponame>`

3. Navigate to "Settings" > "Pages" > "Build and deployment"

4. Change the "Source" to GitHub Actions. Here you can choose between deploying a website with Jekyll or statically. For this website, we chose static deployment. Consider Jekyll if you wish to publish a blog.

5. Now you can create an `index.html` file in your repository and it will publish to `https://<username>.github.io/<reponame>`

## Serving the Website Locally

You may find just opening `index.html` in your browser doesn't work properly. For example, if you have any JavaScript which reads other files, your browser may block this. Instead, you will need to run a local http server. Here is one way of doing this:

1. Install `node.js`
   
   E.g. `conda install nodejs`

2. Install the `http-server` package

    `npm install http-server -g`

3. Run command `http-server` in your website repo

4. Go to browser and type `localhost:8080`

If you are using a website generator (see below) then it likely has its own way of launching a local server to test and develop your site.

## Advanced Website Building

This repository covers creating a simple, one-page website. However, if you want to write a blog or manage multiple pages you should consider a static website generator. Choosing this may require your own experimentation or research. For example,

- [Jekyll](https://jekyllrb.com/) (supported by GitHub pages)
- [Hugo](https://gohugo.io/)
- [Astro](https://astro.build) 
- [Zola](www.getzola.org)

Theses are often command-line scripts which build your site from a set of input files and templates. To deploy them on GitHub pages, you should make use of [GitHub Actions](https://docs.github.com/en/actions). You can search for relevant actions on the [GitHub Marketplace](https://github.com/marketplace) and sort by popularity to find what you want.

If you don't want to start from scratch, search GitHub for template repositories which will include the relevant GitHub Actions to build and deploy your website. Browsing [GitHub Topics](https://github.com/topics) can help in finding these templates. For example, the topic [jekyll-theme](https://github.com/topics/jekyll-theme) has many popular open-source Jekyll themes to explore. Find one with usage instructions and get started.

## Alternatives to GitHub Pages

Here are a few alternatives for website hosting/building which do not require coding,

- Wordpress.org (free) - open source builder (not for hosting)
- Wordpress.com (free/paid) - based on the Wordpress builder with free/paid hosting plans
- Squarespace (paid) - website building and hosting
