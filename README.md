# academic-website

Guide to building an academic website.

1. Follow create instructions at [pages.github.com](https://pages.github.com/) to the base repository for your website. It should be called `<username>.github.io`.

2. To create a static HTML5 website, you can start from scratch or download a template from e.g.

   - [HTML5 UP](https://html5up.net)

3. Clone your repository,
   
   ```bash
   git clone https://github.com/<username>/<username>.github.io
   ```

4. Copy the contents of an HTML5 template into your repository

   - E.g. this site was made with the [Strata](https://html5up.net/strata) template

5. Open `index.html` locally in a text editor and in a browser

6. Make changes to `index.html` and refresh your browser. See what effect the changes have.

If you have already created `<username>.github.io` and want to deploy a new repository to GitHub pages:

1. Create the repository called `<reponame>`

2. Go to the repository "Settings" tab at `https://github.com/<username>/<reponame>`

3. Navigate to "Settings" > "Pages" > "Build and deployment"

4. Change the "Source" to GitHub Actions. Here you can choose between deploying a website with Jekyll or statically. For this website, we chose static deployment. Consider Jekyll if you wish to publish a blog.

5. Now you can create an `index.html` file in your repository and it will publish to `<username>.github.io/<reponame>`

