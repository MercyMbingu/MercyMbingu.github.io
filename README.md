---
layout: "page"
title: Tutorial
permalink: /readme
---

# STATIC WEBSITE FORMATTING AND HOSTING 
---

## PURPOSE

1. To describe the practical steps of how to host and format a resume using Markdown, a Markdown editor, Github Pages, and Jekyll.
2. Relate the practical steps in (1) to the general principles of current Technical writing, as explained in Andrew Etter's book Modern Technical Writing


## PREREQUISITES

- You will need a resume to work with
- You will also need a [Github account](https://github.com/) to host your resume on


*More resources:*

* [Markdown tutorial](https://www.markdowntutorial.com/)
* [Etter, Andrew. Modern Technical Writing](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS)
  * This book is also available with a *Scribd* account.
* [Jekyll tutorial](https://youtube.com/playlist?list=PLLAZ4kZ9dFpOPV5C5Ay0pHaa0RJFhcmcB)


## INSTRUCTIONS

Hosting your resume on Github pages is far easier than it sounds. To begin, have your resume ready! 


### Define your audience

Take time to restructure your resume towards the particular job you are applying to, or your general field of interest. This includes:
1. Identifying the audience
2. Identify the venue
3. State the purpose
4. Determine a desired reaction
5. Note the tone and vocabulary that best suits your audience


### Make Static Websites
Static websites are a simple way to present your documentation to others. To make one:
1. Download your preferred static website generator. I will be using [Jekyll](https://jekyllrb.com/docs/installation/)
2. Open your command prompt and change to the directory you wish to work in.
3. Start by typing "*jekyll new <filename>*" to create a folder for all the files supporting your site. Jekyll will automatically creating some base files and actually create the site.
4. Change into the new directory specified by *<filename>*.
5. To view the actual site, type "bundle exec jekyll serve"
 * Look at the 'server address' value to know which port your site is being hosted on.
 * Open your desired browser and type "localhost:<port>" to view



### Use Distributed Version Control
Once you have your static site up and running on your local device, consider hosting it on a Distributed Version Control (DVC) such as Github. To do so, fire up your command line, move to the directory with all the necessary source code and key in the following commands:
1. *git init*
	Start off by initializing the current directory as a repository on Github
2. *git checkout -b gh-pages*
	This will switch to a new github pages branch
3. *git status*
	This is an optional step To view what files have already been committed to the branch versus those that have not in the current directory
4. *git add .* 
	If no prior commits had been made, this command will upload all files in the directory to the Github branch. If you were only looking to add a specific file, use "*git add <filename>*"
5. *git commit -m "'<comment>'"*
	This command ideally publishes the files you have added to the branch. If the dicumentation was to be worked on in collaboration with others, they would now be able to see the changes you have made.
* If this was your first trial at linking your local server to Github, the previous command may be unsuccessful because your identity is unknown. To remedy this, run:
  * git config --global user.email "you@example.com"
  * git config --global user.name "Your Name"
- Now try (4) again
6. *git remote add origin '<https://github.com/'<username>'/'<repositoryname>'.git>*
	In order to view your website on a browser, type this to add the URL to the alias "origin"
7. *git push origin gh-pages*
	This command will sync local commits with the repository branch to ensure your documents are up to date.


 Other git commands can be found [here](https://education.github.com/git-cheat-sheet-education.pdf).




	
Having your documentation available on a DVC makes it easily accessible to developers. In the case of your resume, it will be right by your projects that could be relevant to demonstrate some of the skills you may have mentioned. 




## AUTHORS AND ACKNOWLEDGEMENTS

 I would like acknowledge Andrew Etter for the commendable writing of the book "Modern Technical Writing". This book has proven to me that technical writing is far less intimidating than I thought prior to reading it.
  
 I would also like to appreciate my group members for helping with peer editing this README thereby making the final copy render more seamless.


## *FAQs*

- _Why host a static website?_
Static websites are simple to create, require almost no resources and are portable to almost every software application. Their diversity will allow you to share your document (in this case resume) publicly with minimal dependencies and allow you to keep everyone with an up-to-date version of your documentation.

- _Why is my resume not showing up after I change a theme?_ 
- Sometimes a theme may not have some of the same layouts you may have defined from the previous theme. Go into the new theme's documentation to check this and change accordingly.



