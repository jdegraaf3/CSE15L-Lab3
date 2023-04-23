
## Lab Report 2
![Image](Screenshot(17).png) (server screenshot) & (compilation screen shot).

The method that is first called when I compile and run my program is "start." The most relevant arguement to this class is "port," this arguement is taken when we run the program and say "java NumberServer 3020," 3020 is passed as the port arguement. It can be seen above what is done with the port number... we get our link with our given port number in it!

Here's what it looks like when we first tap the link:
![Image](login.png) (blank page)

Here's the process of adding a message to the blank board:
![Image](tryingCommands1.png) (add-message?s=Hello)
![Image](tryingCommands2.png) (loading back the board)

Now here's what happens when we want to add another message:
![Image](tryingCommands1.png) (add-message?s=How are you)
![Image](tryingCommands2.png) (loading back the board)

After looking at this, you must be thinking, this guy has to be a master coder and a genious server creator! But it is much simpler than it looks, take a look at my code below and I will discuss wht is going on.
![Image](tryingCommands1.png) (StringServer code)

When first initiating the server we get a blank page. This happens because in the "String" method the first if statement checks to see if the arguement "url" has a slash at the end of it. In this case our url arguement is "localhost:3020," but if you notice there is no slash at the end, well technically there is, it is inferred! If I were to just highlight and copy what is in the search bar and paste it with no edits, you get: http://localhost:3020/. Notice the Slash! So our a String method first checks if the url has a slash at the end by getting its path and currently the only part of the path is the slash. So the if statement runs. First we set a local variable named "string_to_print" to a string that is nothing, we do this so that each time we want to add a new message to the board, we clear the old message from what we may have added to string_to_print.
