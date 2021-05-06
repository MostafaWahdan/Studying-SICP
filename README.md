# What is this?

This is a repository I'm using to track my progress as I read and study [Structure and Interpretation of Computer Programming](https://archive.org/details/ucberkeley-webcast-PL3E89002AA9B9879E?sort=titleSorter) (a.k.a. SICP), a legendary computer science book that uses Scheme, a minimalistic dialect of the programming language Lisp, to explore fundamental principles of abstraction.

# What is your setup for running Lisp code?

I'm using Windows 10 OS as my main operating system and for the course I run WSL2 Ubuntu 20.04.2 LTS. I spent the best part of two days setting up everything to be able to follow along with the book's examples and excercises. 

+ I followed [this](https://youtu.be/IL7Jd9rjgrM) tutorial to setup WSL2 on my machine. It gets into how to create a GUI interface too, but that won't be needed for the purposes of this setup.
+ Once I had Ubuntu up and running, I tried multiple variations of Scheme, the language used in the book and the course. Tried Drracket's simply-scheme and MIT-scheme which were recommended by most but faced a bit of trouble running some of the lecture programs. Eventually, I used [this](https://github.com/bzliu94/cs61a_fa07/blob/master/README.md) guide to install STk-simply, which is the same compiler used in the lectures, hence, it got me exactly the same output for all the lecture programs.
+ So at this point, I have STk-simply running a REPL interface. Still what I don't have is an integration between the compiler and a text editor so that I can edit larger programs and run them in the repl.
+ For that, I chose emacs as my text editor. Wasn't straight forward as it was the first time I deal with it, had to learn couple of shortcuts to get along.
+ Last but not least; needed to set the integration between emacs and STk's scheme. Had to twirl a bit searching for how to set that one up and eventually, thank to [this](https://www-users.cs.umn.edu/~gini/1901-07s/emacs_scheme/) article, one line of code did the magic. Just had to add this line `(set-variable (quote scheme-program-name) "stk")` to "~/.emacs.d/init.el"


I recently came across [this](https://teachyourselfcs.com/) simplified roadmap for studying Computer Science. The first subject on the list is programming.

Now, It could feel a bit like a downgrade to study programming if you've been introduced to more high-level packages that can do magic with just a few lines of code. However, for someone like me who has never been formally introduced to CS, I knew that it would be worth the time to learn more about the basics, especially that the resource recommended for learning about programming, is known to be the world's best CS book.

So, the knowledge presented in the book is in a sense ageless as it dives into different concepts such as black-box abstraction and conventional interfaces directed at managing complexity.

Just finished the first two lectures and already had a couple of aha moments. Also had to set up my machine so that I can run Scheme, the programming language used in the course, which is a dialect of the programming language Lisp.

Now, Studying Brian Harvey's, Spring 2011, lectures. Can be found [here](https://archive.org/details/ucberkeley-webcast-PL3E89002AA9B9879E?sort=titleSorter) and keeping track of my progress using [this](https://github.com/MostafaWahdan/Studying-SICP/) Github repo. and below is a summary of what it took me to be able to run the same compiler being used in the course which was no easy task at all.

Followed this tutorial to set up WSL2 on my machine. It gets into how to create a GUI interface too, but that won't be needed for the purposes of this setup.
Once I had Ubuntu up and running, I tried multiple variations of Scheme, the language used in the book, and the course. Tried Drracket's simply-scheme and MIT-scheme which were recommended by most but faced a bit of trouble running some of the lecture programs. Eventually, I used this guide to install STk-simply, which is the same compiler used in the lectures, hence, it got me exactly the same output for all the lecture programs.
So at this point, I have STk-simply running a REPL interface. Still what I don't have is an integration between the compiler and a text editor so that I can edit larger programs and run them in the REPL.
For that, I chose emacs as my text editor. Wasn't straightforward as it was the first time I deal with it, had to learn a couple of shortcuts to get along.
Last but not least; needed to set the integration between emacs and STk's scheme. Had to twirl a bit searching for how to set that one up and eventually, thanks to this article, one line of code did the magic. Just had to add this line (set-variable (quote scheme-program-name) "stk") to "~/.emacs.d/init.el"
