## For next session we want to 

* put what we have in the test script in the pod label 

* maybe move the repo to our team organisation 


## .Git
We went through the .git directory - witch basically stores all the git information. it is hidden since there in noting one needs to change. To see the hidden directories or files one can do a ls -a in the terminal and then cd into the directory of choice. 


## Gems
To build the gem there is a lib directory where the main code is that builds the program. There is also a Spec directory where all the test files are located. A Gem usually has a lib and a spec and then a Gemfile and a gemspec


## Yaml 

Next thing we did was to look up yaml conversion since yaml don’t have support for comments. 

We are going to use gsub to replace the string with the pod to be able to insert the spec as a comment. 
To do that we use regular expression (regex). 
Regular expression is a language to describe grammar. it describes the structure. 
Regular expression helps to define a search in a less specific way. 

## Some regex syntax:

^.*

^ means beginning of the line 
. means any character 
* means whatever comes before the star could come one ore multiple times 

everything within parantesis () is a group 
referens to group $1
referens to group $2

regular expresions starts with a / and ends with a /


(#{pod}) - the hash and the curly braces lets us grab the value in the variable pod 

backslash backslash 1 - means the first group 

only a hash (#) - means a comment
a hash and curly brases (#{description}) - use the value in var description 
\n - new line
\1\\2 - first group and second group 

group 1 is to create ….
group 2 is to fetch the value of the variable description 


To learn more and to try out regular expression there is an app for Mac called 
Patterns; it enables you to play around with regular expression. 

regex.com is a web app for the same thing


## Some Ruby syntax

a = ‘hello’

#{a} - means include the variable 
that is string interpolation 
\(a) - does the same thing in swift 


## Other useful command line stuff


chmod - means change mode

the man command

man shows the manual page 

man chmod 

man man

man ls 

man chmod
