# Sitekick Templates for Argeweb

## HTML templates
Templates can be added to the `html` folder located in the project folder. (for example: `landingpage/html`)
Standard templates are:

* Header (`header.html`)
* Footer (`footer.html`)
* Page template (`page.html`)

The templates must be build using standard HTML5 and Jinja2 template tags. 
See [Jinja2 docs](https://jinja.palletsprojects.com/en/2.10.x/).
Within these templates you can use sub templates using the Jinja2 inheritance structure.

## CSS
CSS can be written in a file located in the `css` folder. The template structure will be included in the docker image
upon build. The Angular based front-end will try to load the `index.css` file. These files are the entry
point for any arbitrary CSS or JS. 

## JS
External Javascript is *not* supported for security reasons.

## images
Images can just be added to the images folder and be referred to in the html templates.

## Dynamic images
Dynamic images (images with personalised content) can be placed in the `personalised_images` folder. In that folder 
PNG's can be placed acting like a frame to render page screenshots in. Every PNG should be accompanied by a json file
stating the location and size of a `mobile` or `desktop` screenshot.
