# Joanne McGowan Art Website 

This is a static website which is used for displaying and selling artwork for Joanne McGowan. Github user: jmcgowanart, Email: jmcgowan1@hotmail.co.uk. 

It is comprised of an index.html, contact.html, as well as css, js and img folders. It is made using Bootstrap and the relevant Bootsrap files resides in the css and js folders of the project.

---
## Things to note...

### formspree
The contact page needed to be set up in a static way to take advantage of githubs free hosting service (i.e. cannot use PHP). The solution is formspree.io which allows you to send data to their URL, which then gets routed to an email address of your choice... no PHP, Javascript or sign-up required!

You simply connect it to your form like so...

    <form action="https://formspree.io/jmcgowan1@hotmail.co.uk" method="POST">

In order for this to work you need to add a 'name' attritbute to each input tag.


### is-flex class
The 'is-flex' class which can be seen in the stylesheet is used to make sure all columns are identical size... as sometimes with Bootstrap, the columns can appear at different heights and can be quite annoying to fix. 


### Git Command Line 

In order to set up the project for use with git on the command line, I needed to run the below commands in order to change the login from my original kainos account, to the jmcgowan1 account...

    git config user.name jmcgowan1
    git config user.email jmcgowan1@hotmail.co.uk

Only when you go to push the code up to the repo does it ask you for the password associated with the github account. 

---

