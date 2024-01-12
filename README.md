# latex-voice-in: Voice In Plus commands for LaTeX

## Introduction
This repo contains voice commands about LaTeX for the automated speech recognition software Voice In Plus.
Voice In Plus is a Google Chrome extension.
It only works in Google Chrome at this time.
It works in the Overleaf web service that supports the academic writing in LaTeX in the web browser.
I also use it in the text area of 754words.com, although this website does not render the LaTeX.

The utilization of these custom commands requires a subscription to Voice In Plus.
These commands can be used in the text area of most websites and web mail programs opened in Google Chrome.
They might be useful during the drafting of e-mails and grant reviews in secured web sites.

## Usage
After the commands have been uploaded, you can utilize them immediately.
I toggle Voice In on and off by using a custom keyboard shortcut: option-L.
I then dictate the command.
See the documentation for the Voice In plug-in to learn how to configure keyboard shortcuts.

## Installation
Each command is paired with the inserted text on a single line in of a comma separated value file (latex.csv).
Equations, code snippets, and so on that span multiple lines are placed inside of double quotes.
Use the **Bulk Add** button in Voice In Plus to upload these commands into your collection of custom commands.
Existing voice commands will be overwritten, so there has no problem with duplicates when pasting in an updated version of the CSV file.

## Contents of the latex.csv

- lists (font sizes, )
- templates for lists: itemized, enumberated, description, checklists
- templates for floats: figures, tables, code blocks, equations with captions
- templates for tables of various row by column sizes.
- templates for slides with figures, tables, bullet lists
- beamer slideshow preamble

## Related repos
See [Voice Computing section of landing page](https://github.com/MooersLab/MooersLab?tab=readme-ov-file#voice-computing).
At a minimum, you will want to include the library of contractions so that these can be eliminated from your formal prose.
You probably do not want to gunk up your set of custom commands with my Global collection of commands.
Hence, the need for a standalone repository of LaTeX related commands.

## Rules for developing voice commands

### Pick word combinations rarely used in normal prose
The basic rule for developing a voice command is to pick a word combination that is very unlikely to be used in one's prose.
This choice can avoid the accidental insertion of an unintended set of words.

### Pick word combinations that do not contain other commands
If you pick a word combination with a subset of words already assigned to another command, the commands will collide, and you will not get the intended effect.
It is better to pick a synonym for the new command than include the old one.

### Use verbs are prefixes

- Use the verb "insert" in front of the name for the computer code or equation that I want to insert.
- Use the verb "expand" to expand acronyms.
- Use the verb "list" to insert a list of items.
- Use the phrase "url for" to insert the url for a website.

### Test the commands
Like other forms of computer code, test the Voice In commands to ensure you get the intended effect.
The speed with which you vocalize a command has a significant impact.
You may find that you have to verbalize the command at high speed to avoid inserting just the first word of the command rather than the entire command.

### Keep handy the URL to the site for uploading commands
I add commands to my account several times a day.
I keep handy a link to the URL to the site for uploading commands into my account in a my custom built home page called index.html.
I keep the link to the command page on the top line next to my links to other frequently used links like that one to Canvas for my lectures, the project page on Overleaf, 750words.com, Outlook web mail, gmail, and my GitHub and Codeberg repos.

## Contributions are welcome
This project can benefit all NIH grant reviewers.
It should be a community project.
Make a pull request, post a issue, or send me e-mail with additions in csv format.
