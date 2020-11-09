## About Simple Plate

Simple plate was a project created to test and evolve my abilities as a front-end developer.

The project idea is a webpage for cooking recipes. The project's prototype can be [found here] (https://www.figma.com/file/E6xlazw52ICbowNMpNclc8/Untitled?node-id=0%3A1).

The idea and design of the project came from my friend Lucas Credie, a front-end developer, and CEO of Colored Bite.



#### Challenges faced:

As my first front-end project from zero, the callenge of this project was to create a responsive webpage (desktop only), getting data from an external source, like from an API.

As second objectives, there was the development of my knowledge in HTML, CSS and Javascript, and how they combine together to create a responsive webpage.

#### A brief summary of the solution

1. The first challenge was to get the information from an external source. As the project is simple, consisting only of a static webpage, data could not be retrieved by a JSON file. Instead, I've used a variable with a list of Javascript objects, from an external JS file (plates.js).

Data is then treated by a map function, that gets from each plate (js object) the necessary information, and put it in the right spot.

2. The second challenge was to show every plate in the menu bar (left), and to make it selectable to the user, showing the desired plate's info in the main section (right). 

For this, a second function (select_plate) was created:
 - it gets every element inside the "main-plate" div and gives it the "display: none" attribute;
 - it passes through every plate in the menu bar and withdraw the " active" from the class name;
 - it gets the current plate id and changes its main section div with the "display: block" attribute;
 - it adds to the plate menu a tag class name " active";

#### Further modifications

Although the project's main challenge was accomplished, there are some details that still needs work:

- main navbar styling, such as the bottom border's shadow;
- plate's time and serves description in the main section, where image and text are offset;
- ingredients list could be better showed;
- webpage responsiveness to width change (mobile platforms);
