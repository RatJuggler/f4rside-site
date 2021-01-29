# f4rside-site

The F4rside website.

Based on the Stellar template by [HTML5 UP](https://html5up.net/).

### Development

`npm` targets available during development:

- start - runs a development server so that you can see changes to the static files as they are made.
- build - runs a deployment build (experimental, not integrated with docker build).

### Testing

A Docker file is available to create an image for testing with the static files served using my [Nginx golden image](https://github.com/RatJuggler/my-production-docker-build).

- Create an image with: `docker build -f docker/nginx/Dockerfile -t f4side-site .`

  Then run with: `docker run -d -p 8080:80 f4side-site`

  Content will be available at: `http://localhost:8080`

### Full Application

A docker-compose configuration is also available to build, tag and run the image:

    docker-compose up -d

---

Stellar by HTML5 UP

html5up.net | @ajlkn

Free for personal and commercial use under the CCA 3.0 license (html5up.net/license)


Say hello to Stellar, a slick little one-pager with a super vibrant color palette (which
I guess you can always tone down if it's a little too vibrant for you), a "sticky" in-page
nav bar (powered by my Scrollex plugin), a separate generic page template (just in case
you need one), and an assortment of pre-styled elements.

Demo images* courtesy of Unsplash, a radtastic collection of CC0 (public domain) images
you can use for pretty much whatever.

(* = not included)

AJ
aj@lkn.io | @ajlkn


Credits:

	Demo Images:
		Unsplash (unsplash.com)

	Icons:
		Font Awesome (fontawesome.io)

	Other:
		jQuery (jquery.com)
		Scrollex (github.com/ajlkn/jquery.scrollex)
		Responsive Tools (github.com/ajlkn/responsive-tools)
		