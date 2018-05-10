# CSP-GRAMMAR
This repository contains [CSP](https://en.wikipedia.org/wiki/Communicating_sequential_processes) BNF grammar for antlr v4.

## How install ANTLR:
1. Download antlr [here](http://www.antlr.org/)
2. Put `antlr.jar` at `C:\antlr\`.
3. Add/Create a `C:\antlr\antlr.jar` path to `CLASSPATH` variable.  
   - **OBS** : if you have problem like "Can't load 'grammar name' as lexer or parser", set a path like this `.;C:\antlr\antlr.jar`.
4. Append `C:\antlr\;` path to PATH variable.
5. Create `antlr.bat` and `grun.bat` and put at `C:\antlr\`
   - Creating `antlr.bat` file:
     - In this file enter `java org.antlr.v4.Tool %*`, `v4` because i use antlr version 4.7
   - Creating `grun.bat` file:
     - In this file enter `java org.antlr.v4.runtime.misc.TestRig %*`, `v4` because i use antlr version 4.7
     
**OBS** if you have problems go [here](http://www.antlr.org/) or [here](https://levlaz.org/setting-up-antlr4-on-windows/).

## How to use:
 Into folder that contains `Csp.g4` file run this code:
 ```
 antlr Csp.g4 -visitor
 javac *.java
 grun Csp spec -gui <filename>.csp
 ```
 
 ## Contact
 igor.duarte@ccc.ufcg.edu.br
