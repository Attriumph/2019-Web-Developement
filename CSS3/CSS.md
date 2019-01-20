# CSS

### Notes:

* cascading means that it always takes the selector that is at the end.
* in box model, width and height are for content

## Color 

* rgb means red green blue, which can be used by the form of "rgb(255,255,255)"
* also, we can use rgb hex by the form of "#AA3456"
* In addition, there is a rgba, which can change the opacity of the color, a is from 0 to 1
* a good website for color is paletton.com

## CSS Selector

* class, id, * , element selector
* "element1 element2" VS "element1, element2" , "element1 + element2" VS "element1 > element2"
  * "h2 p" means that I want select all 'p's that are inside 'h2'.(inside means all, not just the direct kids)
  * "h2, p" means that both h2 and p elements should follow this style 
  * "h2 > p"  means to select all 'p's - all paragraphs that have a parent of 'h2'. (must be their direct kids)
  * "h2 + p" is says select any 'p' element that is exactly after an 'h2' element

* Three things affect which seletor win out in the cascade:
  * Specificity: how specific is your selector -- we can use speficicity calculator
        CSS Specificity Scoring
         inline style > inner style > external style
            score distribution:
            - HTML tag Element - One
            - Class - Ten
            - ID - Hundred
            - Inline Styles - Thousand
  * Importance:
  * Source order: link source order

## Font

* for font-family, if the name is mutiple words, we need use qutation marks.
* common attributes: line-height, font-style, font-weight, font-family
* Ways to  make sure that a user always sees the same font on a website:
  - 1. One way is to actually include a font file that you have on your computer with all your website files.
  - 2. use google font

## Critical Render Path

## Flexbox

* Good way to pratice it :http://flexboxfroggy.com/

## CSS3 

- Transition and transforom: Good place to learn](https://robots.thoughtbot.com/transitions-and-transforms)
- Place to see attributes if support can be found [browser support]( https://www.w3schools.com/csSref/css3_browsersupport.asp) and [can I use](https://www.w3schools.com/csSref/css3_browsersupport.asp)

## CSS Grid 
1. Common properties for container:
    use "display: grid;" in container
    - grid-gap: 20px;
    - grid-template-columns: 300px 300px 300px;
    - grid-template-columns: 300px 300px 300px;
    - grid-template-columns: 300px 300px 1fr;
    - grid-template-columns: 300px 1fr 1fr;
    - grid-template-columns: 1fr 1fr 1fr;
    - grid-template-columns: repeat(3, 1fr); /*how many times to repeat what*/
    - grid-template-columns: auto 1fr 1fr; /*auto = max size of content*/
    - grid-template-rows: 1fr 1fr 1fr;
    - grid-template-columns: repeat(auto-fill, 200px); 
    - grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
    - justify-items: end;
    - align-items: end;
2. Common properties for chidren
    
    - grid-column: span 2; /*high number will cause it to create extra grids even if we didn't tell it*/
    - grid-row: span 2;
    - grid-column-start: 2;
    - grid-column-end: 4;
    - grid-column: 2 / 4;
    - grid-column: 2 / -1; /* span it to the last track */
    - grid-row: 2 / -1; /*but you need to define rows in the container*/
    - justify-self: end;
    - align-self: end;
[Good link](http://grid.malven.co/)