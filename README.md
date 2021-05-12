# Quizzler  

A trivia GUI app that pulls questions and answers from the opentdb.com api.  

## Setup  

The code is ready to go! You can either open this code in an IDE such as PyCharm or the command line terminal:

```bash  
python main.py
```  

## How To Play

<link rel="stylesheet" href="https://github.com/jNembhard/Quizzler/blob/masterstyles.css">

<body>
  <table>
    <tr>
      <td> <img src="https://github.com/jNembhard/Quizzler/blob/master/Quizzler.gif" width="200" height="300"></td>
      <td>
        <ul>
          <li> Running main.py will start the trivia game (An interactive GUI).</li>
          <li> You can click the "Check Mark" to answer True or the "X" button to answer False for each question. </li>
          <li> The game's screen background will flash "Green" for "Correct" answers and Red for "Incorrect" answers.</li>
          <li> The game is set to 10 questions, which can be edited if needed in the data.py file. </li>
          <li>After the game is finished, the screen reads "You've reached the end of the quiz!"</li>
          <li>Score is updated at the top of the screen. </li>
          <li>To exit the game simply close the window.</li>
        </ul>
      </td>
    </tr>
  </table>
</body>

<br />


##  .py Files

* data.py
	* Sets the amount of  trivia questions and type of questions to be answered (True or False).
	* Requests trivia information from the opentdb.com api.
* main.py
	*  Starts the Quizzler game and opens a new window for the GUI application
	* When the game is finished prints to the console:
		```bash
		You've completed the quiz!
		Your final score was: your_score/number_of_questions
		```

* question_model.py
	*  Creates the Question class.
	*  Initializes q_text and q_answer.
* quiz_brain.py
	*  Creates the QuizBrain class.
	*  Checks the available questions in a list, moves through each question, and updates the player's score until the game is finished.
* ui.py
	* Creates the QuizInterface class.
	* The GUI object displayed to the user.
	* User can click the "Check Mark", or the "X" buttons to answer True or False for each question.
	* The screen changes color based on answer (Green = Correct, Red = Incorrect).
