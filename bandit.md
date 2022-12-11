# Level 0
ssh bandit0@bandit.labs.overthewire.org -p 2220

# Level 0 -> 1
the aim of this level is to find the password in the file called readme
ls<br>
cat readme<br>
ssh bandit1@bandit.labs.overthewire.org -p 2220<br>
ls is used to list the files<br>
cat is used to see the contents in the file<br>
password:NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL<br>

# Level 1 -> 2
the aim of this level is to find the password in the home directory
ssh bandit2@bandit.labs.overthewire.org -p 2220<br>
ls<br>
cat ./-<br>
ls is used to list the files<br>
cat is used to see the contents in the  file<br>
password:rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi<br>

# Level 2 -> 3
the aim of this level is to find the password from  spaces in this filename located in the home directory
ls<br>
cat "spaces in this filename<br>
ls is used to list the files<br>
cat is used to see the contents in the  file<br>
password:aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG<br>

# Level 3 -> 4
the aim of this level is to find the password which is stored in a hidden file in the inhere directory.
ls<br>
cd inhere<br>
ls -a<br>
cat .hidden<br>
ls is used to list the files<br>
cat is used to see the contents in the  file<br>
cd is used for change the directory<br>
ls -a to list all the files with hiddenfiles<br>
password:2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe<br>

# Level 4 -> 5
the aim of this level is to find the password which is in  inhere directory which is human readible
ls<br>
cd inhere<br>
file *<br>
file ./*<br>
cat ./-file07<br>
ls is used to list the files<br>
cat is used to see the contents in the  file<br>
file is used to know what type of file is it <br>
password:lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR<br>

# Level 5 -> 6
the aim of this level is to find the password  from inhere directory using the given prop
ls<br>
cd inhere<br>
ls<br>
ls -al * | grep -B 10 1033<br>
cat maybehere07/.file2<br>
ls is used to list the files<br>
cat is used to see the contents in the  file<br>
ls -al is to listing the files in detail<br>
password:P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU<br>

# Level 6 -> 7
the aim of this level is to find the password which is there some where in the given files
cd ../..<br>
find ./ -group bandit6 -user bandit7 -size 33c<br>
found  ./var/lib/dpkg/info/bandit7.password<br>
cat ./var/lib/dpkg/info/bandit7.password<br>
cd is used to change the directory<br>
find is used to used to filter objects in the file system. <br>
cat is used to see the content in the file<br>
password:z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S<br>

# Level 7 -> 8
the aim of this level is to find the password in the file data.txt next to the word millionth
cat data.txt | grep millionth<br>
cat is used to see the content in the file<br>
password:TESKZC0XvTetK0S9xNwm25STk5iWrBvP<br>

# Level 8 -> 9
the aim of this level is to find the password data.txt which is only one line of text
ls<br>
sort data.txt | uniq -u<br>
ls is used <br>
ls is used to list the files<br>
password:EN632PlfYiZbn3PhVK3XOGSlNInNE00t<br>

# Level 9 -> 10
the aim of this level is to find the password which is in  data.txt
ls<br>
cat data.txt | grep "="<br>
strings data.txt<br>
ls is used to list the files<br>
cat is used to see the content in the file<br>
strings is used to  to return the string characters into files.<br>
password:G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s<br>

# Level 10 -> 11
the aim of this level is to find the password which is in data.txt and use base64
ls<br>
cat data.txt<br>
base64 -d data.txt<br>
ls is used to list the files<br>
cat is used to see the content in the file<br>
base64 is used to convert the biniary to text<br>
password:6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM<br>
# Level 11 -> 12
the aim of this level is to find the password in data.txt
ls<br>
cat data.txt<br>
used CyberChef cipher to decode ROT13<br>
https://gchq.github.io/CyberChef/#recipe=ROT13(true,true,false,13)<br>
ls is used to list the files<br>
cat is used to see the content in the file<br>
password:JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv<br>


