# Flash Cards

[Live Site](https://carlokruger.github.io/flashcards/)

## Stage 1/3: Setting up
### Description
First, you have to come up with the topic for your memory board. When selecting a theme to work with, remember that your questions and answers shouldn’t be too long. Flashcards can be used as an educational tool for a wide variety of tasks, from learning foreign words and scientific terms to memorizing the birthday dates of your new friends. We chose to make geography themed flashcards that can help you memorize the countries' capitals. You can join us with this idea using a list of national capitals on Wiki, or find another theme that interests you.

Once you have chosen your topic of interest, edit the given HTML code. Add a suitable title for your memory-board and nine <div> elements with question terms (in our case, countries).

### Objectives
1. Make an appropriate title using a h1 element
2. Create a div with the question term for each of the nine cards

### Example
The resulting web page should look like something like this:
![webpage](https://ucarecdn.com/96deadba-f61a-4d6d-b3a5-b48a3bb376cc/)

## Stage 2/3: Design
### Description
You got to the most creative part of the project: design! It's time to work out what your web-page should look like. You can make the decisions as you go, draw a tentative plan on a paper, or even use a design app like Figma. Feel free to express your creativity, though there are some restrictions: since projects are about learning, restrictions are necessary for educational and testing purposes.

Don't forget to add a CSS file to the src folder and include a link to it in HTML; otherwise, the added styles will not apply.

First of all, let's design our flashcards. Set the size of divs with questions (notice: the cards are square), add color to the background, round the corners if you want, and position the text inside. Then form a table from the cards. We recommend using the following model of a page and CSS properties grid/flex.
![grid design](https://ucarecdn.com/0ebb6172-7cbd-4433-a840-bc2b9bb2650f/)


Set the background for the element that contains all the cards and the title. We used the picture of the world map, but you can make a solid background if you prefer.

As a final touch, change the fonts of the title and the text on your flashcards.

Be careful, don't use extra elements without need.

### Objectives
1. Make a set of square flash cards.
2. Set the background for the cards and the whole page using the CSS property background-image/background-color.
3. Position the cards using the CSS property grid/flex so they make a 3x3 table.
4. Set the fonts for the text.

### Example
The result of this stage should look something like this:
![finished design](https://ucarecdn.com/693b0b58-fdad-4cee-91fb-8b632a75d082/)

## Stage 3/3: On the flip side
### Description
Your flashcards look beautiful, but something important is still missing. The advantage of flashcards is that they contain answers on the back side so that you can check yourself. For each card, let's create the flip side with the answer (in our case, the capital), which will appear when the user hovers the cursor over the card.

CSS animations are a lot of fun: they are beautiful and not too difficult to implement even for beginners. CSS provides a great variety of effects that you can choose from, and the best option for flashcards is probably flip animation.

To implement the effect, you can either go through our explanation, watch the Youtube [tutorial on flipping card animation](https://www.youtube.com/watch?v=SdC0DDdT_rM), or do both.

If you refer to the tutorial, note: for some browsers the code provided there may not work correctly. You might see the back inscription when the card is flipped; to fix this, add <i>backface-visibility: hidden</i> to the parent of the front and back divs.
It's easy to understand how to make the flip animation if you imagine that you have to make a flashcard from three pieces of paper, which represent correspondent divs:
![3 cards](https://ucarecdn.com/afb9ead0-249d-47ab-8b89-4627e8e565bd/)


To glue the back side correctly, you need to flip it. Use the <i>transform</i> property. The papers would look like this if you could see the text through the paper:
![reversed back](https://ucarecdn.com/434105aa-cff5-453f-a01b-91eed8b56e1f/)


Place all the layers in the correct order. You can use z-index for this.
![stacked cards](https://ucarecdn.com/96b4ae53-9d3d-4caa-af3a-168a86073fc5/)


It's easy to place papers one on top of the other, but it's a bit tricky with divs. Here, you will need to work with positioning and the backface-visibility property.
![stacked](https://ucarecdn.com/724889b7-6a94-4143-8f37-befe8981909f/)

You can flip the resulting paper card by hand, but for virtual cards, you'll use a cursor. Wrap your card in a container div and implement the logic: if you hover on the container, the card inside will be flipped. Here, you will need to work with the properties transition and transform.

Finally, add styles to the back side of your flashcards, and you are all set!

### Objectives
Make the answer on the back side appear when the user hovers over the card.

### Example
The final result of your project will look something like this:

![result](https://ucarecdn.com/170970bc-f84f-4631-b53f-75357f3f7099/)