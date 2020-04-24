## Check is the command executed successfully or not
```
if [[ "$?" == "0" ]];then
  echo "Successfully executed"
else
  echo "Failed"
fi

```


## Converting the case of the String:
```
name='learning Shell scripting'
echo ">>> Input"
echo $name
echo ">>> UPPERCASE"
echo "${name^^}"
echo ">>> LOWERCASE"
echo "${name,,}"
echo ">>> First character to UpperCase"
echo ${name^l}
echo ">>> First character and first word starts with 's' to UpperCase"
echo ${name^s}
echo ">>> First character starts with 's' to UpperCase"
echo ${name^^s)}
```
#### Output
```
>>> Input
learning Shell scripting
>>> UPPERCASE
LEARNING SHELL SCRIPTING
>>> LOWERCASE
learning shell scripting
>>> First character to UpperCase
Learning Shell scripting
>>> First character and first word starts with 's' to UpperCase
learning Shell scripting
>>> First character starts with 's' to UpperCase
learning Shell scripting
```

## Passing command line arguments while executing script:
```
#!/bin/bash
read -p "Enter any value = " num
number=${num^}
echo "Your entered $number."
```
#### Output
```
$ sh test.sh
Enter any value = 343
Your entered 343.
```
