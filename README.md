![Version](https://img.shields.io/static/v1?label=latex-voice-in&message=0.2.1&color=brightcolor)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)


# latex-voice-in: Voice In Plus commands for LaTeX

## Introduction
This repository contains voice commands about LaTeX for the automated speech recognition software Voice In Plus.
Voice In Plus is a Google Chrome extension.
It only works in Google Chrome and Microsoft Edge at this time.
It depends on the Speech-to-Text API of these two web browsers.

Both APIs suffered from degradation of service in mid-March 2024.
They stopped applying proper capitalization of the first word of each sentence.
Until this service is improved, consider using your operating system's Speech-to-Text software.

The Mac Dictation program on Intel Macs sends the soundwaves to a central Apple server, so there is a latency issue. 
The software also does not stay active for more than four sentences.
It also does not tolerate the intervention by the user with the mouse cursor to make minor edits while the software is active.
This advanced feature of the Voice In software is one of many advantages over the Mac Dictation software.
The Mac Dictation software also does not support text replacements like Voice In.

Voice In works in the Overleaf web service that supports academic writing in LaTeX in the web browser.
I also use it in the text area of 750words.com, although this website does not render the LaTeX.

The utilization of these custom commands requires a subscription to Voice In Plus.
These commands can be used in the text area of most websites and webmail programs opened in Google Chrome.
They might be helpful during the drafting of e-mails and grant reviews on secured websites.

## Usage
You can utilize the commands immediately after they have been uploaded.
I toggle Voice In on and off by using a custom keyboard shortcut: option-L.
I then dictate the command.
See the Voice In plug-in documentation to learn how to configure keyboard shortcuts.

## Installation
Each command is paired with the inserted text on a single line in a comma-separated value file (latex.csv).
Equations, code snippets, and so on that span multiple lines are placed inside double quotes.
You can upload these commands into your collection of custom commands using the **Bulk Add** button in Voice In Plus.
Existing voice commands will be overwritten, so there is no problem with duplicates when pasting in an updated CSV file version.

## Contents of the latex.csv

- lists (font sizes, )
- templates for lists: itemized, enumerated, description, checklists
- templates for floats: figures, tables, code blocks, equations with captions
- captioned code blocks for the following pygments-supported languages: cpp, c, R, bash, dot, gnuplot, graphviz, java, javascript, markdown, restructuredtext, mathematica, python, pycon, common-lisp, elisp, clojure, clojurescript, make, cmake, fortran, html, css, latex, nim, bugs, stan, jags, r, rd, rconsole, cython, numpy, sas, stata, rust, slurm, zsh, tsch, text, sqlite3, yaml, julia, jlcon, scheme, matlab, matlabsession, octave, scilab, ocaml, reasonml, applescript, rust, ruby, lua, sed, xml, awk, vim
- templates for tables of various row by column sizes.
- templates for slides with figures, tables, bullet lists
- beamer slideshow preamble


## Related repositories
See [Voice Computing section of landing page](https://github.com/MooersLab/MooersLab?tab=readme-ov-file#voice-computing).
You will want to include the library of contractions at a minimum to eliminate these from your formal prose.
You may not want to gunk up your set of custom commands with my Global collection of commands.
Hence, there is a need for a standalone repository of LaTeX-related commands.

## Rules for developing voice commands

### Pick word combinations rarely used in normal prose
The basic rule for developing a voice command is to pick a word combination that is very unlikely to be used in one's prose.
This choice can avoid the accidental insertion of an unintended set of words.

### Pick word combinations that do not contain other commands
If you pick a word combination with a subset of words already assigned to another command, the commands will collide, and you will not get the intended effect.
It is better to pick a synonym for the new command than include the old one.

### Use verbs are prefixes

- Use the verb "insert" before the name of LaTeX code to insert.
- Use the verb "expand" to expand acronyms and to expand someone's first name to their full name.
- Use the verb "list" to insert a list of items.
- Use the verb "display" before the name of an equation to insert the equation in display mode.
- Use a verb in "inline" before the name of an equation to insert the equation in a sentence.
- Use the phrase "url for" to insert the URL for a website.
- Use the phrase "cite" followed by whatever phrase you used to refer to a specific paper or book to insert its corresponding cite key.
- Use the verb "email" followed by the name of a list of email addresses to send a message to a list of email addresses.


### Test the commands
Like other forms of computer code, test the Voice In commands to ensure you get the intended effect.
The speed with which you vocalize a command has a significant impact.
You may have to verbalize the command quickly to avoid inserting the first word rather than the entire command.

### Keep the URL to the site for uploading commands
I add commands to my account several times a day.
I keep handy a link to the site's URL for uploading commands into my account on my custom-built home page, index.html.
I keep the link to the command page on the top line next to my links to other frequently used links like that one to Canvas for my lectures, the project page on Overleaf, 750words.com, Outlook web mail, gmail, and my GitHub and Codeberg repos.

## Contributions are welcome
It should be a community project.
Make a pull request, post an issue, or send me an e-mail with additions in CSV format.

## Update history
|Version      | Changes                                                                                                                                    | Date                 |
|:-----------:|:------------------------------------------------------------------------------------------------------------------------------------------:|:--------------------:|
| Version 0.2 |  Added badges and update table                                                                                                             | 2024 April 13        |
| Version 0.2.1 |  Added to list verbs in the README.md file.  Added funding.                                                                              | 2024 May 7           |
| Version 0.2.2 |  Minor edits to the README.md to improve readability.                                                                                    | 2024 June 7          |

## Funding sources
- NIH: R01 CA242845, R01 AI088011
- NIH: P30 CA225520 (PI: R. Mannel); P20GM103640 and P30GM145423 (PI: A. West)

