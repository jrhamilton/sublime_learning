##Sublime Learning in Rails!
<a href="https://codeclimate.com/github/Bw00d/sublime_learning">![Code Climate](https://codeclimate.com/github/Bw00d/sublime_learning.png)</a>

###Epicodus "Build anything you want" exercise.

This is an application for practicing Sublime Text 2 keyboard shortcuts.
####Status

* I am able to create lessons.  Each lesson has a name, chapter id, content(which is inputted as markdown and retrieved with the <a href="https://github.com/vmg/redcarpet">redcarpet</a> gem so it can be styled), an editable code block(also markdown), and an answer code block which will be used to compare the result of the user input.
* The <a heref="http://codemirror.net/">codemirror editor</a> is embedded and will allow the user to practice editing the editable code block.
* I am able to add a Sublime Text keyboard binding and use it in the editor.
* I am able to test edited code against answer code and return an alert or notice to the user depending on whether or not their input is correct.
* I can assign the cursor to a specific line for each lesson
* User authentication and validation complete.


####Todo

* Make a consolidated js file of all the relevant key bindings.
* Write js to count keystrokes to test for efficiency.
* Research whether or not I can just edit the vim keybindings instead of chaining methods to make Sublime keybindings.
* Change response functionality so that user does not have to reset after every attempt. 
* Update to secure versions of Rails and Ruby.

####Usage

It is easy to get started building lessons. There is no new lesson link so navigate to the lessons/new to create a new lesson. At this time there is also no authentication to worry about. 


The content, editable_code, and answer <strong>must</strong> be entered as markdown. Make certain to use two space for newline.

The edited code and the answer have to be exactly the same to past the test. 

####Keybindings
**Note** Currently keybindings only work on Mac.
* delete line :  shft+ctrl+k
* delete to end of line : ctrl+k
* indent :  dmc+] !note: the indent() only indent from cursor. blockIndent() is the method that should move the entire line, however, it does not work.
* unindent :  cmd+[
* swap line up : ctrl+cmd+up
* swap line down : ctrl+cmd+down
* duplicate line down : shift+cmd+d
* toggle comment: cmd+/
* toggle block comment : cmd+opt+/ !NOT WORKING!
