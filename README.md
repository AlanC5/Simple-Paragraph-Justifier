# Simple-Paragraph-Justifier
Accept lines of text from user and parses based on user input (width of line) The width represents the amount of characters (including spaces and non-letters)

If the width is not perfect, then adjustments will be made to the line. 

Adjustments can include additional spaces and moving the next word on to the next line. If there is more than one space in the line, then all additional spaces will be divided as evenly as possible across the various spots. 

# Example
```
Enter text, empty return will quit the input
> Hello my name is Alan!      
> This will adjust the length of the paragraph based on the width of one line.
> 
Enter the width of text: 13
|-------------|
|Hello my name|
|is Alan! This|
|will   adjust|
|the length of|
|the paragraph|
|based  on the|
|width  of one|
|line.        |
|-------------|
Enter the width of text: 14
|--------------|
|Hello  my name|
|is  Alan! This|
|will    adjust|
|the  length of|
|the  paragraph|
|based  on  the|
|width  of  one|
|line.         |
|--------------|
Enter the width of text: 20
|--------------------|
|Hello   my  name  is|
|Alan!    This   will|
|adjust the length of|
|the  paragraph based|
|on  the width of one|
|line.               |
|--------------------|
```