thought of having two layers of objects.

the first a bigObject that holds all the smaller objects inside it. 


either {

each small object should includes 
a single index from all the input arrays

so... bigObject[0]
is the first small object...

and the first small object looks like

// an example of what the first small object in the bigObject may look like

firstPossibleSmallObjXxample = {
countries : countries[0],
CorrectAnswer : correctCounter[0]
boolCorrect = false;
userGuess = prompt('whatever the user puts in for an answer, either yes or no),


var x = 'access to a method that can check if userGuess === CorrectAnswer and if it doesset boolCorrect to equal true.';

}


or || or || or

each small object should just be the contents of each of those arrays

secondPossibleExampleSmallObjExample = {
countries : countries,
CorrectAnswer : correctAnswer;
// boolCorrect : an array of all the boolCorrects that have accumulated each time the user guesses correctly;

// if could be a function that returns the boolCorrect at index[i]

// correctCounter: could be a function that accumulates each time a bool is set true, or an array that gets pushed into when true,
}

}


maybe best would be to have each the each way would have pros and cons 
but I want objects in objects in the first place so that I can call everything through one single . notation access

examples 

does bigObj.firstSmallObj.correctanswer = bigObj.firstSmallObj.userGues ?

if so set bigObj.firstSmallobj.boolTruth = true from a defualt of hardcoded false.

do any of the small objects include userGuess?

How many smallobjects have their boolTruth === true, append that return to total bigobject totalcorrect

So i can call methods through dot notation to that be called on any of the small objects or their contents.

a simple method that you can call on a set of questions and itll return a this.big or small object tracker of the user response. Thatll be passed to boolTruth checkers, as arguments alongside the right answer arguments.

like a simple method question asker that takes a set of questions, answers as arguments, compares them and alter the appropriate this.properties, like this.bigObject or this.smallObject boolTruth. 

an alert method that can alert all the correct answers at the end of the guessing game if we didn't want to interupt the game. 

And now thinking it'd be better to branch here, one branch should continue on as I am, the split branch simplifies to pre made smalle objects, like

firstObj = {

country : 'Canada',
correctAnswer : 'yes',
boolCorrect : false,
userGuess : prompt('have I been to' + this.country),
attempts : [],
correctMessage : 'yep, ive been to Canada',
wrongMessage : 'sorry, guess again',
hints : ['maple syrup', 'hockey','moose'],

}

firstObj.prototype.askerFunction = {
    if (if userGuess.includes(correctAnswer)){
    this.boolCorrect = true;
    this.attempts++;
    }

that sort of thing.  


... ok, in simpleObjectBranch i now have firstObj.userGuess call a function that simply prompts them and returns their response using this.country

something to consider is that i think userGuess automatically will call this function, so maybe I could protect this through a clozure? so that it is only called when I want? in other words when I --- firstObj.userGuess --- then it calls askerFunction
  


On the 17th and 18th I continued to work on the functionality of my about me guessing game, i've solved good chunks of the logic and now need to organize that logic in Javascript. And I need to link it up to some basic html and css.



