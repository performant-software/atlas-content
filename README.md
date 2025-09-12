# Core Data CMS content for Atlas

## Building the website

The following steps will result in a statically-generated version of Core Data Places for Atlas:

* `git checkout` the `master` branch of https://github.com/performant-software/core-data-places
* Place the `.env` file provided by Performant in the top-level directory.
* Run `npm run build`. This will take several minutes as it fetches data from FairData and generates the static routes.
* The output will be in the `dist` directory, with `index.html` as its entry point. Serve this however you prefer to serve static websites.
