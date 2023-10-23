# The Tea Cozy 

This was a small project from CodeCademy where you are challened to recreate [this static website] with the information shown on the website and using Flexbox. I deviated slightly from the instructions as I prefer this dark mode (`#282828`) color compared to straight up black (`#000000`). I also did not add opacity of 0.9. for the same reason.  

## Challenges
There was a few times I got stuck. 
1. The ribbon. I dind't struggle with making a ribbon, but there were small parts about that didn't initially turn out the way it was supposed to. For example, the white bottom border was not stretching till the very end on the left of the page. After some research I found out I needed to just add `left: 0;` 
2. The background of the page. When you try scroll out of the page, you usually see the same color as the general page color. In my case, it was black `#000000`. Initially, I used black with opacity of 0.9 to get the darkmode color I wanted. 
`* {
    color: seashell;
    font-family: Helvetica;
    color: black;
    opacity: 0.9;
}` 
or 
`html {
    color: seashell;
    font-family: Helvetica;
    color: black;
    opacity: 0.9;
}` 
However, that only worked for everything within the HTML tag. So, when I was scrolling beyond the ribbon, the color was black, while rest of the page had an opacity of 0.9. After some googling, I found out that it was the opacity that caused this problem. My solution to this problem was to find a hex color with light balck color that I liked, which ended up being `#282828`. As I am writing this md file, I found out that I could have used `rgba(0,0,0,0.9)` to solve the problem and keep the initial color I chose. 
3. While the ribbon went otherwise smooth, the "Our mission" section went smooth, and the "Tea of the Month" went smooth (once I figured out I needed to use `display: inline-flex; flex-wrap: wrap;`), the "Location" section and the Footer was a harder nut to crack. 
    - The Location section doesn't look that hard, but in my case, the subtitle addresses did not want to align vertically in the of the picture. I defined the height and put `align-items: center;`, but whatever I tried, it did not work. Therefore, I chose a scuffed solution which was to manually push the H2 title and addresses down manually until it looked good. I did this my putting `position: relative;` and pushing the elements from the top. 
    - The background picture for the Location section is soomed in compared to the instructions. I don't know what is causing it as I put the height to 500px as requested. This wasn't a major problem to be, so I decided to let it be. 
    - Lastly, the Footer section was overlapping with the Location section. I had no idea why this happened, and still don't, but solved again the problem by putting `position: relative;` and pushing the elements from the top. 


## Imporvements
1. I believe the CSS file can be organised better. I could make sections inside the CSS file to organise the code better. 
2. The CSS code has many improvements. I know there are better ways to solve my problem that makes the website better and reproducible for other projects. I know the problems that occured in the Location and Footer section are self inflicted, but I can't identify what affected the elements to act the way it did. 


## Final notes
I am overall happy with the project. I am proud I managed to (almost) recreate the website fully with some minor color twists. I am also proud that I solved the problems that came up by myself through Googling, experimenting with code, and utilising CodeCademy's course (although the solutions to these problems can be improved.) Happy I finished the project and looking forward to the next one!