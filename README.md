# Fleet Coding Challenge

> Welcome to the Fleet Coding Challenge!


## Overview

To complete this challenge, you will need to write a simple [React](https://facebook.github.io/react/) web app, and provide us the source files to be built.

The purpose of this challenge is to assess your **skills and approach to composing a simple web app** given a set of screens and an API feed.  We will also assess the **generated HTML, CSS, and JS** output.

This challenge is expected to take about 2-4 hours.


## The Challenge

It's pretty simple. Using the provided screens as a reference, you'll need to build a set of React components to render the app.  You'll also need to request a JSON feed, filter that data, and use the relevant fields.

Although this is a basic exercise, we'll be looking for **simple, well-designed and tested code** in the submission.


## Details

You will need to build the following 3 pages with React:

* A "Home" page
* An "Ocean Provider" page
* An "Air Provider" page
* A "Custom Broker" page

The deployable solution should be built in a folder named **`dist`** with an entry point file of **`index.html`**.

Please create components for each part of the page (eg. header, content, footer, etc).
Assets are provided in the `assets` folder.

The pages should also be usable on mobile and tablet devices.

You can assume that you do not have to support legacy browsers without features such as `fetch` or `flexbox`.

View screens here: [SCREENS](https://invis.io/62DXI51HS)

### "Home" Page

Refer to the [screens/1-home.jpg](./screens/1-home.jpg) screen.

This will be your `index.html` screen.

You will need to display 2 tiles, which link to the "Ocean Providers" page, the "Air Providers" page and the "Customs Brokers" page..


### "Ocean Providers", "Air Providers" and "Custom Broker Providers" Pages

Refer to the [screens/2-series.jpg](./screens/2-series.jpg) and [screens/3-movies.jpg](./screens/3-movies.jpg) screens.

For each page you will need to fetch the JSON feed [feed/sample.json](./feed/sample.json), then:

* Display the first 21 `providers`
* Where the entry has a `yearStarted` attribute value >= `2010`
* Sorted by the `companyName` attribute value in ascending alphanumeric order

For the "Ocean Providers" page filter on:

* Where the entry has a `type` attribute value of `ocean`

For the "Air Providers" page filter on:

* Where the entry has a `type` attribute value of `air`

For the "Custom Brokers Providers" page filter on:

* Where the entry has a `type` attribute value of `customBroker`

The attributes you should use to display the entries are:

* `providers`
* `images` → `Company Logo` → `url`

You will also need to handle the loading and error states, of fetching the JSON feed:

* "Loading" state [screens/1.1-loading.jpg](./screens/1.1-loading.jpg)
* "Error" state [screens/1.2-error.jpg](./screens/1.2-error.jpg)


## FAQ

### What language, framework, build tool... should I use?

You may use whatever you like as long as the solution is built using [React](https://facebook.github.io/react/).

### What should I include with my source code?

Please include a `README` with setup instructions, and any tests or other documentation you created as part of your solution.

Also, add the following info to your `README`:

* How did you decide which technologies to use as part of your solution?
* Are there any improvements you could make to your submission?
* What would you do differently if you were allocated more time?


## Useful Links

* [Bitbucket](https://bitbucket.org/) - Source code hosting, with free private repositories for small teams.
* [Google Fonts - Raleway](https://fonts.google.com/?selection.family=Raleway)
* [React](https://facebook.github.io/react/)
