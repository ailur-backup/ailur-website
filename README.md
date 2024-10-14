# ailur-website

The Ailur website Wordpress source code

To use:
- Download the latest continuous release to "bootstrap" the site
- Start a local webserver and run it at port 80
- Open your Wordpress instance **on your local machine** to import the XML
- Use a plugin like Auto Upload Images to move the bootstrapped images to your Wordpress instance

This is because the Wordpress XML file does **not** bundle images. Our Wordpress instance is therefore configured to fetch all images from itself, which exported as localhost, meaning you must move all the "localhost" images over to your instance.

FOSS Wordpress sites are a pain :P