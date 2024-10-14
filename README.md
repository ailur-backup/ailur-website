# ailur-website

The Ailur website Wordpress source code

To use, you can do one of two things:

Option 1 (not reliant on ailur.dev)
- Download the latest continuous release to "bootstrap" the site
- Start a local webserver and run it at port 80
- Open your Wordpress instance **on your local machine** to import the XML
- Use a plugin like Auto Upload Images to move the bootstrapped images to your Wordpress instance

Option 2 (requires an active internet connection)
- Run `chmod +x ./search-and-replace.sh`
- Run `./search-and-replace.sh`
- Import the XML in any Wordpress instance
- Use a plugin like Auto Upload Images to move the bootstrapped images to your Wordpress instance


This roundabout method is needed because the Wordpress XML file does **not** bundle images.

Our Wordpress instance is configured to fetch all images from itself, which exported as localhost, meaning you must move all the "localhost" images over to your instance.

`./search-and-replace.sh` replaces any instances of images to links to (the ailur website)[https://ailur.dev], allowing you to bootstrap the server from our active production server instead.

FOSS Wordpress sites are a pain :P