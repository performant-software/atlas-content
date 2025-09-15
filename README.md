# Core Data CMS content for Atlas

## Deploying the website

* Performant will run the build process and supply UQAM with a `dist.zip` file containing the static website.
* Unzip the file and serve its static contents however you prefer (e.g. nginx, Apache, etc.)

## Updating the website

The steps for updating are the same as above. Performant will run the build process and deliver an updated `dist.zip` file to you.

Since the website is statically generated, content updates will not immediately appear on the site and will require a rebuild.

## Adding new projects

If you wish to add new projects in the future, Performant will need to update the search indexing script and the website config file.

## Building the website

Let Performant know if you would prefer to build the site yourself. This process is fairly simple, but it requires a recent version of Node and a `.env` file from Performant.

The following steps will result in a statically-generated version of Core Data Places for Atlas:

* Check out the `master` branch of https://github.com/performant-software/core-data-places
* Place the `.env` file provided by Performant in the top-level directory.
* Run `npm run build`. This will take several minutes as it fetches data from FairData and generates the static routes.
* The output will be in the `dist` directory, with `index.html` as its entry point. Serve this however you prefer to serve static websites.
