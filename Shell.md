# Shell
## Exist code
``$?``: exit status of last command
``0``: normal, ``1``: error

## Process
``$$``: process ID of the current shell instance

## IF Conditions
### String Comparison
``str1 = str2``
``str1 != str2``
``-n str1``: Returns ``true`` if the string is not ``null``
``-z str1``: Returns ``true`` if the string is ``null``
### Num Comparison
``expr1 -eq expr2`` - ``ne``, ``gt``, ``ge``, ``lt``, ``le``, ``! expr``
### File Conditionals
``-d file``: True if the file is a directory
``-e file``: True if the file exists(-f is generally used)
``-f file``: True if the string is a file

## Iteration Loop
````
apps="app1 app2 app3"
for app in ${apps} do
    echo "app name ${app}"
done
# Output
#> app name app1
#> app name app2
#> app name app3
````

## Utilities
### find
- Iterate through all folders under a directory
````
appList=`find /app/myDir -maxdepth 1 -mindepth 1`
for appHome in ${appList}; do
    echo ${appHome}
done
````
- Find files modified since n minutes ago
``find -mmin +n``

### basename & dirname
|       path    |  dirname  | basename  |
|   ----------- |  -------- |    ------ |
|   "/usr/lib"  |   "/usr"  |   "lib"   |
|   "/usr/"     |   "/"     |   "usr"   |
|   "usr"       |   "."     |   "usr"   |

### rsync
TODO

## Tips
- Ensure last command succeed
````
if [ "$?" -eq 0 ]; then 
    echo "successfull"
else
    echo "ERROR"
fi
````