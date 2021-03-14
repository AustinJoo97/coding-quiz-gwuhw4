# Javascript Code Quiz

This web application is a simple coding quiz game about HTML, CSS, and Javascript sytax that was created using these very languages. 

## Link

## About the Application

The program itself cycles through multiple html divs that are conditionally hidden and shown through css property adjustments. When a user first loads the quiz, they will be presented with a simple screen with the quiz title (rendered using an HTML <h1> tag) and a start button.
  
Upon clicking the start button, the initial html button will become hidden and the first question and answer set will be loaded. There will also be a timer that is visible to the user; starting at 30 seconds, it will continue to decrement until the quiz is over. 

With each question that is rendered to the viewport, a set of answer buttons and a next button, with the prior becoming visible to the user in a random order (to prevent cheating to replicate a real quiz), and each answer option has the ability to change color upon both hovering and focusing to indicate to the user which answer was selected. After selecting an answer, the "next" button can be clicked which will check the selected answer to that which is set in the answerKey object within the JS file. If the wrong answer answer is selected, 3 seconds will be taken from the remaining number of seconds, accelerating the progression of the quiz. If the answer is correct, a currentScore html element will be updated to indicate to the user what their current score is. 

After either the time runs out or the user clicks "submit" after answering the final question, questions and their corresponding answers will not longer render and, instead, the user's final score and an input box will be visible. The input will accept any 2 character string that will be used to save the user's userInitials to localstorage along with the score. 

After saving the score and initials, the user will be taken to a page which will notify the user where in the score-ladder he/she placed as well as rendering the top 5 highest scorers of the quiz. This top 5 list will be generated by interating and rendering the first 5 score objects saved to the localstorage.hiScore key's value which will hold an array of score:userInitials objects that were sorted in descending order based on score. 

## Screenshots
