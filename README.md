# draft

github + [appveyor](https://appveyor.com) + [pandoc](https://pandoc.org): your own little markdown to .docx online publishing pipeline.

This little repo allows you to:
- edit a text file in markdown, 
- save all your changes in git,
- when you are ready to publish, just tag a release
- and you'll magically get a converted .docx file added to your release.

It works by using appveyor to run pandoc to turn your markdown file into a .docx. 

All of the editing and release process can be done locally in git or online using the github editor.

To get this working for yourself:
- clone the repo
- get an [appveyor](https://appveyor.com) account
- add the repo to your appveyor and edit the appveyor.yml to give it your own github token ([instructions here](https://www.appveyor.com/docs/deployment/github/))
- then do your drafting in the draft.md file (you can use the github online editor for this, or do locally and commit your changes)
- when you are ready to publish, just tag a release (you can do this online by adding a new release in github, or use the git tag command locally)... wait a few moments and an output.docx file should magically appear on that release.
