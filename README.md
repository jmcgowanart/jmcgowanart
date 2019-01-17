# Joanne McGowan Art Website 

This is a static website which is used for displaying and selling artwork for Joanne McGowan. Github username: jmcgowanart, Email: jmcgowan1@hotmail.co.uk. 

It is comprised of an index.html, contact.html and an about.html, as well as css, js and img folders. The site was made using using Bootstrap and the relevant Bootsrap files reside in the css and js folders of the project.

---
## Important things to note within the project...
---

## Formspree
The contact page needed to be set up in a static way to take advantage of githubs free hosting service (i.e. cannot use PHP or server side programming). The solution is formspree.io which allows you to send data to their URL, which then gets routed to an email address of your choice... no PHP, Javascript or sign-up required!

You simply connect it to your form like so...

    <form action="https://formspree.io/jmcgowan1@hotmail.co.uk" method="POST">

In order for this to work you need to add a 'name' attritbute to each input tag, as simple as that.

## Online Payments with Snipcart
Snipcart is a static web solution to taking payments from customers. Eventually snipcart was taken out of this project due to its minimum monthly fee of $10, so it didn't fit the use case... However it is useful to know for future projects. 

You simply include their library at the top of your file, add the 'snipcart-add-item' class to your buy buttons and add certain attributes, like so...

    <button class="snipcart-add-item btn btn-primary btn-lg"
         data-item-id="1"
         data-item-name="As the sun goes down, Ards, Donegal."
         data-item-price="100.00"
         data-item-url="/"
         data-item-description="Oil on board. Selling this piece for £100. Unframed.">
        
         Buy Artwork
    </button>

It's as simple as that. Another alternative is PayPal Business Accounts. 


## is-flex class
The 'is-flex' class which can be seen in the stylesheet is used to make sure that all columns are identical size... as sometimes with Bootstrap, the columns can appear at different heights and can be quite annoying to fix. I needed to use the is-flex class on the footer of this site, to make each column appear flush with one another. 


## Domain Name
The Domain name 'joannemcgowanart.co.uk' was purchased from www.godaddy.com (credentials saved in my LastPass vault). 
Various Records needed to be configured so that the domain would point correctly to the github pages website.
Namely these 4 IP addresses needed to be configured... 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153.
As well as that, a CNAME record needed to be created with the name 'www' and value '@'. This was to ensure users could prefix the address with 'www' also. 

## Git Command Line 

In order to set up the project for use with git on the command line, I needed to run the below commands in order to change the login from my original kainos account, to the jmcgowan1 account...

    git config user.name jmcgowan1
    git config user.email jmcgowan1@hotmail.co.uk

Only when you go to push the code up to the repo does it ask you for the password associated with the github account (also saved in my LastPass vault).

### Sequence of Commands

Here is a refresher of the commands needed to create a new branch off master, then stage our changes locally, before pushing them to the remote repo, and checking out the master branch again. 

    git checkout -b "feature/changingProfilePicture"

    git add .
    
    git commit -m "insert message"

    git push --set-upstream origin feature/changingProfilePic

    git checkout master
    
    git pull

---

