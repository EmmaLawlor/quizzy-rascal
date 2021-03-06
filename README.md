# Quizzy Rascal

![image](https://user-images.githubusercontent.com/84344402/130507807-86dc40fc-00da-4232-acac-4583947160b3.png)

## Author
Emma Lawlor

## Project Overview
Quizzy Rascal is an interactive music trivia quiz. Designed to provide entertainment to the user, the quiz asks 10 random music questions. The quiz is presented in a multiple-choice format, displaying the correct/incorrect answers on submission and keeping track of the user's score at the bottom of the window. The random question is selected from an array of over 20 questions, meaning the round of 10 questions will vary slightly each time the quiz is played, keeping the site interesting for the user. 

The name was chosen as a play on the stage name of English rapper Dizzee Rascal, helping to set a fun and lighthearted tone. 

## Deployed Site
https://emmalawlor.github.io/quizzy-rascal/

## Table of Contents
- [Quizzy Rascal](#quizzy-rascal)
  * [Author](#author)
  * [Project Overview](#project-overview)
  * [Deployed Site](#deployed-site)
  * [Table of Contents](#table-of-contents)
  * [UX](#ux)
    + [Project Goals](#project-goals)
      - [As the Site Owner I Want to:](#as-the-site-owner-i-want-to)
      - [As the Site User I Want to:](#as-the-site-user-i-want-to)
    + [Design Choices](#design-choices)
    + [Wireframes](#wireframes)
    + [Implemented Features](#implemented-features)
    + [Future Features to Implement](#future-features-to-implement)
  * [Testing](#testing)
    + [Validation Testing](#validation-testing)
      - [HTML](#html)
      - [CSS](#css)
      - [JavaScript](#javascript)
    + [Manual Testing](#manual-testing)
    + [Cross Browser and Device Testing](#cross-browser-and-device-testing)
    + [Defects](#defects)
      - [Defects of Note](#defects-of-note)
      - [Outstanding Defects](#outstanding-defects)
    + [Spelling and Grammar](#spelling-and-grammar)
  * [Accessibility](#accessibility)
    + [Lighthouse Audits](#lighthouse-audits)
    + [Keyboard Navigation](#keyboard-navigation)
  * [Deployment](#deployment)
  * [Credits](#credits)
    + [Media](#media)
    + [Content](#content)
    + [Acknowledgements](#acknowledgements)
    + [Thank You](#thank-you)

## UX

### Project Goals
#### As the Site Owner I Want to:
- Present a fun, interactive music quiz to the user.
- Provide the user with instructions/rules for playing the quiz.
- Give feedback to the user when an answer is selected, displaying both correct and incorrect options. 
- Display the user's current score throughout the running of the quiz.

#### As the Site User I Want to:
- Play a fun and easy to use quiz to test music knowledge.
- Progress easily and intuitively through the quiz, with the option of returning to the home screen at any point.
- Be informed whether a chosen answer was correct or incorrect when selected.
- Be aware of current score while progressing through the quiz. 

### Design Choices

- Typography
    - The 'Nova Round' font from [Google Fonts](https://fonts.google.com/specimen/Nova+Round) was used throughout the site.
    
    ![image](https://user-images.githubusercontent.com/84344402/130508625-44e97d2f-e8a0-420b-ac7e-2a407aa2f88c.png)
    
    - A fallback font of cursive was used in case of any browser compatibility issues with chosen fonts.

- Images

    - [Background Image](https://github.com/EmmaLawlor/quizzy-rascal/blob/main/assets/images/music-notes.jpg) of black and white music notes chosen as it is in keeping with the musical theme of the quiz. The same image was used across all pages of the site to maintain a sense of familiarity and to keep the overall layout simple and content-focused. 

![Background Image](documentation/background-image.jpg)

- Colors 

    - Vibrant yellow(#ffff00) ![image](https://user-images.githubusercontent.com/84344402/130504915-71b37849-2d01-4426-a4c3-139674287dd8.png)
 and blue(#0000ff) ![image](https://user-images.githubusercontent.com/84344402/130504866-b10213ee-d192-4533-9b86-4f971e7a2b66.png)
 colors were chosen for the site to maintain the fun feel of the site. 
    - As seen in the wireframes, the Quizzy Rascal heading and sub-heading were originally intended to be blue. 
    - The [WebAIM](https://webaim.org/resources/contrastchecker/) site was used to check the contrast of both colours against a background of black, the predominant colour of the background image. 
    - The blue(#0000ff) color failed the contrast check in terms of accessibility.
    ![image](https://user-images.githubusercontent.com/84344402/130504388-2ec94089-bc58-4f62-a871-5057cdae7aee.png)

    - The yellow(#ffff00) colour passed the contrast check, and so the heading and sub-heading were changed to this font colour to improve visual accessibility. 
    ![image](https://user-images.githubusercontent.com/84344402/130504563-107f846c-a319-4b21-8dc6-8471b95199d4.png)
    
    - Colour codes were taken from [htmlcolorcodes.com](https://htmlcolorcodes.com/)

- Transitions/Animations
    - A fade-in/out effect was applied to the quiz area of the Quiz page to enhance user experience and visual appearance. 
    - When the user selects an answer to the displayed question, the answer button first turns red or green depending on whether the answer was correct/incorrect.
    - The entire quiz container then fades out and fades back in, displaying a new question to the user. 
    - Before adding this fading effect, the divs appeared a little jumpy when displaying a new question. This transition makes the change to a new question appear more seamless. 

### Wireframes
- The wireframes for this project were created using (Balsamiq)[https://balsamiq.com/]
- The Home, Quiz and Results pages were drawn up in mobile, desktop and tablet views. 
- The wireframes helped to map out the basic structure of the site while building the project, however, some style and layout changes were made throughout the development process. 
    - Desktop View: Home, Quiz and Result Pages
    
    ![image](https://user-images.githubusercontent.com/84344402/129425119-0f04b530-abef-4505-88c6-e29fe6add371.png)
    ![image](https://user-images.githubusercontent.com/84344402/131180828-df994e02-3400-4306-8b00-3dfb6b3dba1c.png)
    ![image](https://user-images.githubusercontent.com/84344402/131181007-b7b401da-e47e-4fa8-a8bf-a8c30bf6b94c.png)

    - Mobile View: Home, Quiz and Result Pages
    
    ![image](https://user-images.githubusercontent.com/84344402/129425193-ececaa72-b0bb-4846-bb64-5050ee13e758.png)
    ![image](https://user-images.githubusercontent.com/84344402/131180894-5627eba9-ebeb-4f5b-9c2f-68ec2c16a762.png)
    ![image](https://user-images.githubusercontent.com/84344402/131181089-f8865b15-7a1c-4876-8abe-22fa466b427a.png)

    - Tablet View: Home, Quiz and Result Pages
    
    ![image](https://user-images.githubusercontent.com/84344402/129425052-77deec35-7028-47dd-aa99-06aa311d25ad.png)
    ![image](https://user-images.githubusercontent.com/84344402/131180961-8fefe5ab-a9a6-4cf5-b2fc-a13d3d756de8.png)
    ![image](https://user-images.githubusercontent.com/84344402/131181164-c870ab7a-fa1b-4050-8107-22035e0cdfa0.png)

[Quizzy Rascal Wireframes](https://1drv.ms/b/s!AtrJulJDGsm2pl-VpVw5-fjdsVzS)

### Implemented Features
- Heading & Sub-heading: prominently positioned in the top centre of the window on both the home page and result page. The inclusion of these gives the user a very clear indication of what the site is about. 
-![image](https://user-images.githubusercontent.com/84344402/130509464-64570996-720e-42c8-8078-c3cdcbaf14e4.png)

- Play Button: Located in the centre of the home page, this takes the user straight to the start of their quiz game making the site very easy to navigate.

![image](https://user-images.githubusercontent.com/84344402/130509645-be6459ca-a144-4f25-84c6-a65275381c61.png)

- Rules Modal: Again located in the centre of the home page, the rules button activates a modal that simply describes how to play the quiz and how scoring works. This makes the quiz quite simple for any user to play. The modal also features a play button that takes the user directly to the start of the quiz.
![image](https://user-images.githubusercontent.com/84344402/130509865-b496db37-3062-4213-89b1-9f0ec7fc3586.png)

- Home Link: Featured in the top-left corner of the Quiz page, this house icon acts as a direct link back to the Home page making site navigation simple for the user. 

![image](https://user-images.githubusercontent.com/84344402/130510829-587a73f5-8572-4cd1-86f6-8c839c4a1355.png)

- Audio Control: Located in the top-centre of the Quiz page, this allows the user to control the background music which is available while playing the quiz. The background music can easily be toggled on/off with a simple click of the volume icon. 

![image](https://user-images.githubusercontent.com/84344402/130510957-20956f35-9727-498a-9f6c-b5db90fef763.png)
![image](https://user-images.githubusercontent.com/84344402/130511002-7a103c6b-e4b4-40bf-a278-b07e87375d30.png)

- Score Tracker: Located in the top-right of the quiz page, this keeps track of and prominently displays the user's score throughout the quiz. It increments by 1 point each time a question is answered correctly. 
![image](https://user-images.githubusercontent.com/84344402/130511411-1f578456-49fd-4819-a78c-834f9d67575f.png)

- Quiz Area: Main play area of the quiz page. Question is displayed along with 4 multiple choice answer buttons. User selects their answer by clicking an answer button, which turns green if the answer is correct or red if the answer is incorrect. The quiz then displays the next set of questions/answers after a short delay, up to a maximum of 10 questions.
![image](https://user-images.githubusercontent.com/84344402/130514148-153ec3d4-d373-402a-b493-8036a08d1094.png)

- Result Box: Displayed at the end of the 10 quiz questions, this shows the user their final score for the round. The result box also contains a 'play again' button which takes the user back to the quiz page to start another round of 10 questions, encouraging the user to continue playing the quiz. 
![image](https://user-images.githubusercontent.com/84344402/130514842-e429c537-c848-420e-855d-9b7700bdf902.png)

- 404 Error Page: Included to improve user experience should they encounter a 404 error while using the site. The 404 page is styled in the same colours and font as the rest of the site and features the same background image, maintaining a sense of familiarity should an error occur. The light-hearted error message tells the user that something is "off-key" and prompts them to get back on "the right track" in reference to the musical theme of the site. The page simply features 2 links to allow the user to go back to the home page or directly to start the quiz, keeping the site easy to navigate and user-friendly. 
![image](https://user-images.githubusercontent.com/84344402/131112480-5c1da2eb-11c9-483d-b1ec-8071be3fc810.png)

- No Script: This element was included to cater for the possibility that JavaScript may be disabled on the user's browser. It consists of a simple message informing the user that JavaScript is required in order to play the quiz. The user is also given a link that takes them to a Google search, which will provide instructions on how to enable JavaScript, thus allowing them to progress with the quiz. The Google link opens in a new tab, keeping the user on the Quizzy Rascal site.
![image](https://user-images.githubusercontent.com/84344402/131186628-70f7b4db-efa8-4348-99f6-7a13101603ac.png)

### Future Features to Implement
- Score Board
    - This would allow the user to add their name and score to a leaderboard on the site. 
    - This could keep a record of the top 5 or 10 users and their scores. 

- Extend quiz options
    - Create several music trivia categories based on music genres or decades of music.
    - Add the option of selecting difficulty so the user could answer easy or difficult questions, depending on their music knowledge.

- Enhance CSS
    - Use CSS to help display the focused button on the quiz more clearly when tabbing through the page via the keyboard. 
    - At present the default blue highlight blends with the style of the buttons on the page. 

## Testing

### Validation Testing

#### HTML
All HTML pages of this site were validated using [W3C validator](https://validator.w3.org/)

- The Home page (index.html) returned the following errors
![image](https://user-images.githubusercontent.com/84344402/130333967-e79f0f37-aff4-4638-80aa-0d8a7ee80113.png)
    - This was rectified by removing the button element from both of the links in question, as seen here:
    ![image](https://user-images.githubusercontent.com/84344402/130334266-e42f0e50-e9d4-466a-8d0e-cd3ae2f639a1.png)

    - The links were then styled to resemble buttons using CSS, as shown here:

    ![image](https://user-images.githubusercontent.com/84344402/130334276-4fd86152-43e8-44f0-b971-050c5d2f6a63.png)

    - After making these adjustments, the Home page passed through the validator without any errors or warnings.
    ![image](https://user-images.githubusercontent.com/84344402/130334309-0a850d53-f0e3-4ad6-95ab-f4f3455363e0.png)

- The quiz page passed through the validator with no errors or warnings.
![image](https://user-images.githubusercontent.com/84344402/130334484-4dc4555c-f76c-4c49-be97-905fcfbc3769.png)

- The result page returned the following error:
![image](https://user-images.githubusercontent.com/84344402/130334510-f39a9f75-7760-4135-8dab-f69a6fb746f1.png)
    - As above, on the home page, this was corrected by removing the button element from the play link.
    ![image](https://user-images.githubusercontent.com/84344402/130334541-dbd9c6fe-5c0b-4e1c-a34d-48a0d8a30ea1.png)
    
    - The link was then styled to resemble a button, in keeping with the rest of the site:
    
    ![image](https://user-images.githubusercontent.com/84344402/130334614-98ce6f6c-6f9f-48e1-811b-912f8f41b635.png)

    - The quiz page then passed through the validator with no further errors or warnings:
    ![image](https://user-images.githubusercontent.com/84344402/130334635-cefffa2d-7978-4ae1-8a22-b0ef0e44903c.png)
    
    - The 404 error page passed through the validator with no errors or warnings:
    ![image](https://user-images.githubusercontent.com/84344402/131182420-0f15d563-7c9b-4925-8c3d-9093b336acef.png)

#### CSS
- The CSS file for this was validated using the [W3C Validator](https://jigsaw.w3.org/css-validator/)
- When passed through the validator, the CSS file returned no errors or warnings

![image](https://user-images.githubusercontent.com/84344402/130334711-16930143-fae7-4575-961b-9a7578e95f5d.png)

#### JavaScript
All JavaScript files for this site were validated using [JSHint](https://jshint.com/)
- The script for the Rules modal returned no errors or warnings
![image](https://user-images.githubusercontent.com/84344402/130522884-6aea01f7-83f6-46bc-b465-d78bd1797620.png)

- The file for the quiz page returned the following

![image](https://user-images.githubusercontent.com/84344402/130523014-e1ab75a5-ea8f-44d6-a56d-a0d0633b927a.png)

    - The first issue regarding displayUserResult is due to the file structure of the site. This function is defined in another file and used here, which is not take into account by JSHint.
    - Of the 5 unused variables detected, 3 were deleted from the file (quizBox, answerBtn and result) as they were not used in the project. 
    - The variables checkAnswer and musicControl flagged as undefined as these are called from the HTML page using onclick function. 

- The JavaScript file for the Result page returned no errors or warnings 

![image](https://user-images.githubusercontent.com/84344402/130523108-2eef7482-ea0f-4586-810e-a1f41bbed627.png)

### Manual Testing
Manual testing of all features of the site was carried out on a number of devices and browsers, as detailed in [this document](https://1drv.ms/b/s!AtrJulJDGsm2pgfk5eR_CTdHovEF)

*Preview*
![image](https://user-images.githubusercontent.com/84344402/130518972-c83cbc1b-300c-4617-a4ad-7ea1bb51313d.png)

### Cross Browser and Device Testing
The site was tested across a number of devices and browsers to ensure all elements function correctly and appear as expected. The browsers and devices tested are as follows:

| TOOL / Device                   | BROWSER     | OS         | SCREEN WIDTH  |
|-------------------------------  |-------------|------------|---------------|
| real phone: iPhone8             | safari      | iOs        | XS 375 x 667  |
| real phone: iPhone11            | safari      | iOs        | XS 414 x 896  |
| real phone: samsung galaxy s10  | chrome      | android    | XS 360 x 740  |
| real tablet: ipad Air 2         | safari      | iOs        | M 768 x 1024  |
| real computer: avita laptop     | chrome      | windows 10 | XL 1366 x 768 |
| real computer: avita laptop     | firefox     | windows 10 | XL 1366 x 768 |
| real computer: dell desktop     | chrome      | windows 10 | XL 1920 x 1080|
| dev tools emulator: iPhone5s    | safari      | iOs        | XS 320 x 568  |
| dev tools emulator: ipad pro    | safari      | iOs        | L 1024 x 1366 |
| dev tools emulator: MS lumia550 | edge        | windows    | XS 360 x 640  |

### Defects

#### Defects of Note
- Any defects which occurred during development were tracked using the GitHub Issues section of this repository, which can be found [here](https://github.com/EmmaLawlor/quizzy-rascal/issues).
- Details of each bug were noted as they were discovered, with screenshots taken to demonstrate the problem where possible. 
- The GitHub Issues section allowed for closeout of defects as they were rectified, again using screenshots to show the solution when possible. 

#### Outstanding Defects
- No outstanding defects have been noted. 

### Spelling and Grammar
- The text content of the site was checked for spelling and grammar errors using [Grammarly](https://www.grammarly.com/)

## Accessibility

### Lighthouse Audits
- All 3 HTML pages were tested using Google Chrome's Lighthouse audit function and returned good results in all categories.
 - Home Page
 ![image](https://user-images.githubusercontent.com/84344402/131173141-4dc452ce-2f6b-4067-a6cc-31b607dee99a.png)

 - Quiz Page
 ![image](https://user-images.githubusercontent.com/84344402/131173261-0c9c3996-119e-41a3-ab96-3762c3262778.png)

 - Results Page
 ![image](https://user-images.githubusercontent.com/84344402/131173389-8cde3e3e-04a3-40ca-a57a-d453c5b5646d.png)

### Keyboard Navigation
- Keyboard navigation could be improved by highlighting the button outline better. 
- This was not implemented on the site so as not to deviate from the style of the site. 
- Future development could focus on improving the button highlight using CSS

## Deployment

The site was deployed from its [GitHub Repository](https://github.com/EmmaLawlor/quizzy-rascal) to GitHub Pages using the following steps: 

1. From the Quizzy Rascal repository, select the Settings tab.
![image](https://user-images.githubusercontent.com/84344402/129406799-46c24512-e424-48e3-89b3-5b9a2e3a85c7.png)

2. Select the Pages sub-menu on the left of the page.

![image](https://user-images.githubusercontent.com/84344402/129406863-5eac3c50-1ab5-4b2a-a2eb-a2b4c2f1c53f.png)

3. Under Source, select the main branch and hit save.
![image](https://user-images.githubusercontent.com/84344402/129406956-65bd0e3f-ac1b-45f6-a735-1f6878483654.png)

![image](https://user-images.githubusercontent.com/84344402/129406984-6886c55d-9ea1-4169-a6c1-f590178c32d7.png)

4. Upon saving, the page refreshes to confirm deployment of the site and provides a link to [live site](https://emmalawlor.github.io/quizzy-rascal/)
![image](https://user-images.githubusercontent.com/84344402/129407005-9dad2c38-1f07-46ab-a85b-ccb9e86856fb.png)

## Credits

### Media
- [Background Image](https://github.com/EmmaLawlor/quizzy-rascal/blob/main/assets/images/music-notes.jpg) of black and white music notes, used on all pages taken from [pxhere.com](https://pxhere.com/en/photo/1043482)

- Background music is track "Online Deal", taken from [playonloop](https://www.playonloop.com/freebies-download/)

- House icon for home page link and audio control icons used in quiz pager header all taken from [Font Awesome](https://fontawesome.com/)

![image](https://user-images.githubusercontent.com/84344402/129630296-236f52a2-fb62-406d-97cc-a0bb512b869b.png)
![image](https://user-images.githubusercontent.com/84344402/129630340-74afbddd-315a-4142-84c6-e2cc6f83da98.png)
![image](https://user-images.githubusercontent.com/84344402/129630453-651ab19a-b470-45f5-9007-ee11a1b217b3.png)

- Screenshot of the live site for this write-up created using [AmIResponsive](http://ami.responsivedesign.is/)

### Content
- Trivia content for quiz questions take from [Radio Times](https://www.radiotimes.com/quizzes/pub-quiz-music-round/) and [Thought Catalog](https://thoughtcatalog.com/samantha-newman/2020/04/music-trivia-questions/)

### Acknowledgements
- Favicon created using [favicon.io](https://favicon.io/favicon-converter/)
- Nova Round font imported from [Google Fonts](https://fonts.google.com/specimen/Nova+Round?query=round#glyphs)
- Help sought from W3Schools in creating modal to contain quiz rules. Code adapted and modified from [here](https://www.w3schools.com/howto/howto_css_modals.asp)
- Help in applying click transform effect to buttons from [Geeks for Geeks](https://www.geeksforgeeks.org/how-to-add-a-pressed-effect-on-button-click-in-css/)
- Code for incrementing user's score was adapted from the Code Institute Love Maths walkthrough project
- Help in centering the modal on the screen was sought from [Stack Overflow](https://stackoverflow.com/questions/39627549/how-to-center-modal-to-the-center-of-screen/39636961)
- Help in fixing the size of the background image from [css-tricks.com](https://css-tricks.com/perfect-full-page-background-image/)
- Help with the fade transition on Quiz page was from [css-tricks.com](https://css-tricks.com/almanac/properties/t/transition/)
- Code for window onload event adapted from [W3Schools](https://www.w3schools.com/jsref/event_onload.asp)
- Much help in constructing the basic quiz and JavaScript functions was got from [this tutorial](https://youtu.be/f4fB9Xg2JEY) by [Brian Design](https://www.youtube.com/channel/UCsKsymTY_4BYR-wytLjex7A)
- Readme table of contents created using [https://ecotrust-canada.github.io/markdown-toc/](https://ecotrust-canada.github.io/markdown-toc/)

### Thank You
- Thanks to Code Institute cohort facilitator Kasia for providing advice and learning resources as well as a listening ear, whenever needed. 
- Thank you to the Code Institute tutors who provided such helpful feedback when needed. 
- A huge thank you to my mentor Malia Havlicek for her wisdom, advice and invaluable experience when providing support throughout project development. 
