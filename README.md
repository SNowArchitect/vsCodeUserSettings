# vsCodeUserSnips

Relies on the following extension 

- **Insert Date String:** Insert the current date and time according to configured format.

- **Better Comments:** Improve your code commenting by annotating with alert, informational, TODOs, and more!

- https://github.com/jsynowiec/vscode-insertdatestring

- https://github.com/aaron-bond/better-comments

Unfortunately you can't use anything more than tab stops or variables in snippets so you'll have to enter the title and date/time manually.

You can define snippets for specific languages. To open a snippet file for editing, open User Snippets under File > Preferences (Code > Preferences on Mac OS X) and select the language for which the snippets should appear.

Following example is for Plain Text files.

After opening a snippet file for Plain Text, add following definition:


 {

     "File header": {
     
        "prefix": "header",
        
        "body": [
        
            "title: ${title:Enter title}",
            
            "date: ${date:Insert datetime string (⇧⌘I or Ctrl+Shift+I)}"
            
        ]
        
    }
    
 }
 
Now you can open a new plaintext file, enter header and press Tab. Enter your title and use Insert DateTime command to insert current date and/or time.
