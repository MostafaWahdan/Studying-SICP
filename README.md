# What is this?

This is a repository I'm using to track my progress as I read and study [Structure and Interpretation of Computer Programming](https://archive.org/details/ucberkeley-webcast-PL3E89002AA9B9879E?sort=titleSorter) (a.k.a. SICP), a legendary computer science book that uses Scheme, a minimalistic dialect of the programming language Lisp, to explore fundamental principles of abstraction.

# What is your setup for running Lisp code?

I'm using Windows 10 OS as my main operating system and for the course I run WSL2 Ubuntu 20.04.2 LTS. I spent the best part of two days setting up everything to be able to follow along with the book's examples and excercises. 

+ I followed [this](https://youtu.be/IL7Jd9rjgrM) tutorial to setup WSL2 on my machine. It gets into how to create a GUI interface too, but that won't be needed for the purposes of this setup.
+ Once I had Ubuntu up and running, I tried multiple variations of Scheme, the language used in the book and the course. Tried Drracket's simply-scheme and MIT-scheme which were recommended by most but faced a bit of trouble running some of the lecture programs. Eventually, I used [this](https://github.com/bzliu94/cs61a_fa07/blob/master/README.md) guide to install STk-simply, which is the same compiler used in the lectures, hence, it got me exactly the same output for all the lecture programs.
+ So at this point, I have STk-simply running a REPL interface. Still what I don't have is an integration between the compiler and a text editor so that I can edit larger programs and run them in the repl.
+ For that, I chose emacs as my text editor. Wasn't straight forward as it was the first time I deal with it, had to learn couple of shortcuts to get along.
+ Last but not least; needed to set the integration between emacs and STk's scheme. Had to twirl a bit searching for how to set that one up and eventually, thank to [this](https://www-users.cs.umn.edu/~gini/1901-07s/emacs_scheme/) article, one line of code did the magic. Just had to add this line `(set-variable (quote scheme-program-name) "stk")` to "~/.emacs.d/init.el"
