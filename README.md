# CarouselCSS
A carousel with pure HTML, CSS (no JavaScript needed). Currently there are supported up to 10 Slides per Carousel.

## Installation
To install CarouselCSS, it is sufficient to download the files from GitHub. Afterwards, insert the `carousel.css` into your project.

## Configuration
Configuring CarouselCSS is very simple. Add the carousel.css to your project and then link the carousel.css in your HTML file as follows:  
  
`<link rel="stylesheet" href="path/to/carousel.css">`
  
Make sure to provide the correct path to the `carousel.css` file depending on where you have it stored in your project. If you're unsure about the steps to follow, you can refer to the example in the `index.html` file. Never add your custom code directly to the carousel.css file, and avoid modifying the code there to prevent errors. Instead, you can define your own code in a separate `style.css` file and import it after the `carousel.css` in your HTML file to modify predefined rules such as the carousel size, background colors etc.  

## Usage
After importing the `carousel.css` into your HTML file, you can create a carousel using pure HTML code.

First, create the container for the carousel:

`<div class="carousel">`  
`	...`  
`</div>`  

Next, add a wrapper container inside the carousel:
   
`<div class="carousel">`  
`	<div class="carousel-wrapper">`  
`		...`  
`	</div>`  
`</div>`  
  
Now, add individual slides and their content. In this example, three slides are added, but you can add up to 10 slides:
  
`<div class="carousel">`  
`	<div class="carousel-wrapper">`  
`		<div class="carousel-slide">`  
`           Slide 1`  
`       </div>`  
`		<div class="carousel-slide">`  
`           Slide 2`  
`       </div>`  
`		<div class="carousel-slide">`  
`           Slide 3`  
`       </div>`  
`	</div>`  
`</div>`  

Next, add bullets for carousel navigation. These should be defined before the `carousel-wrapper` and should not be nested in other containers. Make sure to set the first radio button to checked. The `id="carousel-css-slide-1"` should be unique for each radio button and should not be used in any other carousel. Also, make sure to set the value to the corresponding slide, e.g., `slide-1`. The value should always be specified as `slide-x`, where `x` represents the slide number. This value can be reused in other carousels as well.

`<div class="carousel">`  
`   `  
`	<input type="radio" id="carousel-css-slide-1" name="carousel-css" value="slide-1" checked/>`  
`	<input type="radio" id="carousel-css-slide-2" name="carousel-css" value="slide-2"/>`  
`	<input type="radio" id="carousel-css-slide-3" name="carousel-css" value="slide-3"/>`  
`  `   
`	<div class="carousel-wrapper">`  
`		<div class="carousel-slide">`  
`           Slide 1`  
`       </div>`  
`		<div class="carousel-slide">`  
`           Slide 2`  
`       </div>`  
`		<div class="carousel-slide">`  
`           Slide 3`  
`       </div>`  
`	</div>`  
`</div>`  
  
Finally, add navigation arrows to the carousel. These will appear on the left and right sides of the carousel and are optional. Please ensure that you provide the for attribute with the corresponding ID of the radio button.

`<div class="carousel">`  
`   `  
`	<input type="radio" id="carousel-css-slide-1" name="carousel-css" value="slide-1" checked/>`  
`	<input type="radio" id="carousel-css-slide-2" name="carousel-css" value="slide-2"/>`  
`	<input type="radio" id="carousel-css-slide-3" name="carousel-css" value="slide-3"/>`  
`  `  
`	<label for="carousel-css-slide-1" data-value="slide-1"></label>`  
`	<label for="carousel-css-slide-2" data-value="slide-2"></label>`  
`	<label for="carousel-css-slide-3" data-value="slide-3"></label>`  
`  `   
`	<div class="carousel-wrapper">`  
`		<div class="carousel-slide">`  
`           Slide 1`  
`       </div>`  
`		<div class="carousel-slide">`  
`           Slide 2`  
`       </div>`  
`		<div class="carousel-slide">`  
`           Slide 3`  
`       </div>`  
`	</div>`  
`</div>`  

## Requirements
- Text-Editor for editing the code files
- Min. Internet Explorer 11, Firefox 70, Google Chrome 70, Safari 11, Chromium 70

## Contribute
If you want to contribute to the development of this project, feel free to submit pull requests or open issues. Let's make ServerVBS even better together!

## License
This project is licensed under the [MIT License](LICENSE).
