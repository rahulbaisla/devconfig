# Customized Prompt
Add content from CustomizedPrompt.txt to your .zshrc file

OLD_PS1="%F{yellow}%n %d ~ "

```
%F{yellow} - Yellow font color
%n         - Username
%d         - Current directory
```


PS1=$'%B%F{240}${(r:$COLUMNS-20::-:)}%D{%f/%m/%y} %D{%L:%M:%S}\n''%B%F{white}$OLD_PS1%F{white}'
```
%B%F{240} - Bold Grey Font color

${(r:$COLUMNS-20::-:)} - Insert '-' 

%D{%f/%m/%y} %D{%L:%M:%S} - Formatted Date at end of line of dashes

%B%F{white}$OLD_PS1%F{white} - Bold font before Prompt and Normal Font after prompt
````

![Prompt in action](./customized_prompt.png)