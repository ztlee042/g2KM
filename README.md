# g2KM

## MN KM
* Involved Apps: [MarginNote(MN)](), [Notebooks](), [KeyBoard Maestro]().
* Reference: [A video on Bilibili.com]() & [An article on sspai.com]()
* Purpose: I want to exerpt some **key concepts** from the chapters I read on MN to a more condensed app, for which i use Notebooks.

### The .zip file contains three Macros:
### 1-Notebooks New
* This one triggered by hot key in MN, and works in both MN and Notebooks.
* Copy the **content** and **url** of card in MN
* Activate Notebooks, create a new note page for the chapter, and paste the content and url.
### 2-Notebooks Append
For some reasons, there is no such function in Notebooks for Mac, so I create this macro to meet the need.
* This one triggered by hot key in MN, and works in both MN and Notebooks.
* Copy the **content** and **url** of card in MN
* Activate Notebooks, paste the content and url in a *new line*
### 3-2Markdown
The "Coverted to Markdown" function in Notebooks without a hot key, so I use AppleScript to write one for it.
* This one triggered by hot key in Notebooks.
* Covert the .txt file to .md file
* The AppleScript:
```
tell application "System Events"
	tell process "Notebooks"
		click menu "Edit" of menu bar item "Edit" of menu bar 1
		delay 0.3
		click menu item "Convert to Markdown..." of menu "Edit" of menu bar item "Edit" of menu bar 1
	end tell
end tell
```
