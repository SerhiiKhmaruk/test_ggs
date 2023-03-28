##  Basic work with files

- Create directory test1 - mkdir test1

```console
mkdir test
```

- Create file test1.txt inside the test1 directory - touch test1/test1.txt or vim/cat


-   Create copy of folder test1 with name test2 - cp -R test1 test2

-    Delete file test1.txt inside test2 directory - rm -rf test2/test1.txt 

-    Rename test2 folder into directory_without_file - mv test2 directory_without_file

-    Insert 'test1' text into test1/test1.txt file - cat > test1/test1.txt or vim
  test1

-    print the text from the test1/test1.txt file - less test1/test1.txt or cat

-    Insert 'test2' into the end of test1/test1.txt file - echo "test2" >> test1/test1.txt or vim

-    print the text from the test1/test1.txt file - less test1/test1.txt or cat

-    check the size of test1 directory - du -sh test1 or stat 

## Permissions

-   Create test directory and block access for all to it:
-        mkdir khmaruk
-        chmod 000 khmaruk


-   Try to remove that directory:
-        rm -rf khmaruk 
-        I could not open the folder, but I was able to delete it.


-    Create simple script which prints current date. Try to execute it:
-        vim nowdate.sh
-        Let's write command - date
-        Let's add execution rights - chmod +x nowdate.sh
-        Run the script - ./nowdate.sh


## Log checking

-  Count lines in the file test.txt - wc -l file.txt 


-  Show last 3 lines from the test.txt file - tail -3 file.txt


-  Hom many uniq IP addresses accessed the website? - less test.txt | cut -d' ' -f1 | uniq | wc -l


        !!!!!!!!!!!IN PROCESS!!!!!!!!!!!
        Final result may vary.

-  IP address with most requests - less test.txt | cut -d' ' -f1 | sort -t " " -k 1 | uniq -c


-  Top 3 IP addresses by amount of POST requests - 


-  Which IP addresses received 403 error?:
        less test.txt | grep 403 | cut -d' ' -f1 | sort  | uniq -c
        or
        less test.txt | grep 403


- Task with * . Write script to show which pages Google checked from the website - 

## Replace

Replace IP address with most requests on 127.0.0.1 in test.txt file - 
