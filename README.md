# Qeasy - Quick & Easy General knowledge quiz

![amiresponsive](https://user-images.githubusercontent.com/73644304/118357631-1306a080-b573-11eb-8475-e939486eb54a.png)

[Link to the quiz](https://barbirm.github.io/qeasy/index.html)

This is web application for quick test of your general knowledge. Simple styled, with multiple choice answers, to make waiting for the bus shorter. Main features are:
- Interactivness
- Progress counter
- Score counter
- Final result display
 
## UX
 
UX is kept minimalistic to capture the easiness feeling. Your initial options are just either start the quiz or see the instructions. Final page, with your total score display, is just your score - no pass/fail ratios, no score/total - just simple display which will lead you to want to try again.

As the use of the app is quite simple, there was no need for well deffines user stories, as the goal was simply to make the quiz displays and responsivnes to the user input is present.

### Potential future version impovements

Open sourced API is used to generate questions (see Technologies Used section) and even from the quick test of the app, many typos or odd symbols are noticed. This descreases the user expirience, but the value at this moment is higer.

Size of the answer buttons depends on the amount of text it holds which results with variability in sizes - not great user expirience, but the value of leaving it as it is at this moment is higer.

## Design

Colour Scheme
- #2b2d2f (chrysler charcoal grey)
- #f0e68c (khaki)
- #ffff00 (yellow)
- #adff2f (greenyellow)
- #ff0000 (red)
- f5f5f5 (whitesmoke)

Font
- Source code pro, monospace

Wireframes
- [Deskop wireframes available here](https://github.com/barbirm/qeasy/blob/master/Desktop.pdf)
- [Mobile wireframes available here](https://github.com/barbirm/qeasy/blob/master/Smartphone.pdf)
- [Tablet wireframes available here](https://github.com/barbirm/qeasy/blob/master/iPad.pdf)

## Web-site Content

#### Home page (Main Menu)

- Components:
    - Title, logo, descripition 
    - Start button
    - Instructions button

- Features:
    - Can start the quiz by clicking 'Start button'
    - Can start instructions by clicking 'Instructions' button


#### Instructions

- Components:
    - Short instructions
    - Start button
    - Main Menu button
    
- Features:
    - Can start the quiz by clicking 'Start button'
    - Can go back to the Main Menu by clicking 'Main Menu' button

#### Quiz

- Components:
    - Progress text
    - Score counter
    - Question
    - Four option answers
    - Main Menu button

- Features:
    - When starting the quiz by clicking any 'Start' button, first (random) question will be displayed, as well as the four possible answers. API used contains 50 different questions, from different categories, of different difficulty - more than enough while that bus is here.
    - When clicking the selected answer, button colours green if correct or red if incorrect. After quick pause, new question is diplayed.
    - One round of the quiz will have 10 questions displayed.
    - After last (10th) question is answered, final result page is displayed.
    - Throughout the whole lenght of the quiz, at the bottom of the page is 'Main Menu' button, which enables user to go back to the Main Menu page.

#### Final result

- Components:
    - Total score display
    - Play again button
    - Main Menu button

- Features:
    - Total score is displayed when landed on the page.
    - When 'Play again' button is clicked, new round of the quiz starts.
    - When 'Main Menu' button is clicked, Main Menu is displayed.


#### Bugs faced along the way

1. When selecting the answer:
- expected: when user clicks anywhere on the answer button, selection is accepted
- observed: user has to click on text of the answer for selection to be accepted
Fix: Modifing answer paragraph in CSS.

2. When selecting answer to the last question:
- expected: the app navigates to the Final result page
- observed: Error and page cannot be loaded.
Fix: Correcting the path for the Final page's html file 

## Technologies Used

- HTML 5

- CSS 3

- JavaScript

- Bootstrap v4.6.0
    - Used through whole web-site for it's responsive features and styling.

- Font Awesome v5.6.3
    - Used icons to add more character to the footer.

- [Open Trivia Database API generator](https://opentdb.com/api_config.php)
    - Questions for the quiz are obtained from the API generated on this page

- Google Fonts

- Chrome Developer Tools
    - Used for live testing.

- Adobe Photoshop
    - Used to design icon.

- Visual Studio Code
    - Code editor used for project.   

- Git
    - Used for version control by commiting, keeping track on the project and pushing to Github.

- Github
    - Used for storing the project and sharing it.        


- [JQuery](https://jquery.com)
    - The project uses **JQuery** as part of Bootstrap.


## Testing

Due to the lack of the well defined user stories, testing was done to check if the basic stream of the functionality works:
1. Can user launch the quiz?
2. Is quiz displayed?
3. Is there responsivness on the user's input?

#### Website is tested on three different web-browsers:

- Google Chrome:
    - Tested and working perfectly.

- Mozilla Firefox:
    - Tested and working perfectly.

- Microsoft Edge:
    - Tested and working perfectly.

#### Website is tested for fluidity, speed and responsiveness on different devices using Chrome Dev tools:

- Galaxy S5:
    - Tested and working perfectly.

- Pixel 2:
    - Tested and working perfectly.

- Pixel 2 XL:
    - Tested and working perfectly.

- iPhone 5/SE:
    - Tested and working perfectly.

- iPhone 6/7/8:
    - Tested and working perfectly.

- iPhone 6/7/8 Plus:
    - Tested and working perfectly.

- iPhone X:
    - Tested and working perfectly.

- Regular tablet size:
    - Tested and working perfectly.


#### W3 Markup Validator, W3 Jigsaw CSS Validator, JavaScript

- W3 Markup Validator:
    - Tested and corrected all the errors. [Link available here](https://validator.w3.org/nu/?doc=https%3A%2F%2Fbarbirm.github.io%2Fqeasy%2Findex.html)

- W3 Jigsaw CSS Validator:
    - Tested and corrected all the errors. Error on Bootstrap classes left open. [Link available here](https://jigsaw.w3.org/css-validator/validator?uri=https%3A%2F%2Fbarbirm.github.io%2Fqeasy%2Findex.html&profile=css3svg&usermedium=all&warning=1&vextwarning=&lang=en)

- JavaScript
    - Tested by exploring the code in the console in Chrome Developer Tools

## Deployment

Steps for deployment:
1. In the project's repository, click on 'Settings'
2. Go to 'GitHub Pages', and under 'Score' select the branch you want to deploy. In this case, it was 'Master'.
3. Choose the folder to deploy from.
4. Click 'Save', and visit your URL (above 'Source')

Final version of project is uploaded to Github Pages, it can be visited here - [Qeasy](https://barbirm.github.io/qeasy/index.html)

## Credits
- Quiz functionality inspired by [Brian Design YouTube Tutorial](https://www.youtube.com/watch?v=f4fB9Xg2JEY&ab_channel=BrianDesign)
- Self-invoking fade CSS animation [found here](https://stackoverflow.com/questions/11679567/using-css-for-a-fade-in-effect-on-page-load)

### Media
- Icon done by developer 
- Wireframes and screenshot done by developer

### Acknowledgements

- Code Institute team for teaching me necessary skills for the project, guiding me through the course and fully support anythime needed.
