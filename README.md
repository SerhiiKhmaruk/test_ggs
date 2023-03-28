##  Basic work with files

- Create directory test1

```console
mkdir test1
```

- Create file test1.txt inside the test1 directory

```console
touch test1/test1.txt or vim/cat
```

-   Create copy of folder test1 with name test2 

```console
cp -R test1 test2
```

-    Delete file test1.txt inside test2 directory

```console
rm -rf test2/test1.txt 
```

-    Rename test2 folder into directory_without_file

```console
mv test2 directory_without_file
```

-    Insert 'test1' text into test1/test1.txt file

```console
cat > test1/test1.txt or vim
  test1
```

-    print the text from the test1/test1.txt file

```console
less test1/test1.txt or cat
```

-    Insert 'test2' into the end of test1/test1.txt file

```console
echo "test2" >> test1/test1.txt or vim
```

-    print the text from the test1/test1.txt file

```console
less test1/test1.txt or cat
```

-    check the size of test1 directory -

```console
du -sh test1 or stat 
```

## Permissions

-   Create test directory and block access for all to it:

```console
mkdir khmaruk
chmod 000 khmaruk
```

-   Try to remove that directory:

```console
rm -rf khmaruk 
I could not open the folder, but I was able to delete it.
```

-    Create simple script which prints current date. Try to execute it:

```console
vim nowdate.sh
Let's write command - date
Let's add execution rights - chmod +x nowdate.sh
Run the script - ./nowdate.sh
```
  
## Log checking

-  Count lines in the file test.txt

```console
wc -l file.txt 
```

-  Show last 3 lines from the test.txt file

```console
tail -3 file.txt
```

-  Hom many uniq IP addresses accessed the website?

```console
less test.txt | cut -d' ' -f1 | uniq | wc -l
```

# !!!!!!!!!!!IN PROCESS!!!!!!!!!!!
# Final result may vary.

-  IP address with most requests - 

```console
less test.txt | cut -d' ' -f1 | sort -t " " -k 1 | uniq -c
```

-  Top 3 IP addresses by amount of POST requests - 

```console
processing...
```

-  Which IP addresses received 403 error?:

```console
less test.txt | grep 403 | cut -d' ' -f1 | sort  | uniq -c
or
less test.txt | grep 403
```

- Task with * . Write script to show which pages Google checked from the website - 

```console
processing...
```

## Replace

Replace IP address with most requests on 127.0.0.1 in test.txt file 
```console
processing...
```
