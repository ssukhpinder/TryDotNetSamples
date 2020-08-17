# Learning Strings

### Strings 
Try modifying the code so that the console says hello to *your name*, instead of the *world*. For example, I used the *Sukhpinder Singh*. Replace *Sukhpinder Singh* with your name.

``` cs --region strings --source-file .\myapp\Program.cs --project .\myapp\myapp.csproj 
Console.WriteLine("Hello Sukhpinder Singh");
```
### Variables
In programming we want to store values in a container so we can use them later; these are called `variables`.
Let's store your name in a variable, then read the value from that variable when creating the output message. 

``` cs --region variables --source-file .\myapp\Program.cs --project .\myapp\myapp.csproj 
var name = "Sukhpinder singh";
Console.WriteLine("Hello " + name + "!");
```
The first line `var name = "Your Name";` declares a variable, *name* and assigns it a value,`Your Name`. The second line prints out the name.

### String Interpolation
You've been using  `+` to combine variables and constant strings.  There is a cleaner way to do this. 
Start with including a `$` before the opening quotes of the string. Now, place a variable between curly braces `{ variable name}`, and this will tell C# to replace `variable name` with the value of the variable. This is called **string interpolation**. 

``` cs --region interpolation --source-file .\myapp\Program.cs --project .\myapp\myapp.csproj 
var name = "Sukhpinder Singh";
Console.WriteLine($"Hello {name}!");
```
#### Home - [Home](../README.md)
