 Wrote the whatIsHappeningFunction() that lets me see the state change for my question array and I can confirm that each time, the question is indeed spliced from the array. 

Decided to separate one function into two, one handles grabbing a unique question from my array, the other handles displaying it and handling the logic. But maybe those two functions can be cleaned and separated two?

Went ahead and separated it into three separate functions, one to grab a question, one to display it, and one to handle the logic. But the logic function was running into some trouble.

And why? 

The positive and negative conditions were working… but the else condition, if the user enters gibberish causes trouble, it will alert properly but then, to reprompt with that same question was messy. I didn't want to call my randomquestionpicker function again because that would call a new question and I want the current question… so I came up with a current question that gets pushed to an array, !!! But I need to pop that later on… Well anyway I'd recursively called that function in the else statement to call the function again with the user notified their input was valid. And it worked, but the weird thing is that would prompted twice! The first time the prompt still was containing the string entered from the user before, their gibberish input, then the corrected input they type, was correctly entered on the second time. Michael caught this fact with a nice console.log. Which console logged, gibberish, then the correct input. 

Then Michael explained to me that this is an example of advanced JavaScript recursion which I didn't follow 100% but the gist is that the first time of the recursion the state is still in the past, and then on the second time recursion is when the correct input is passed, and then it works.

!!! So the question is how to still recursively call that logic() function but without two passes over, just once… how to do that? And if that's not possible, what's the way to do that as closely as possible to what I have? 





