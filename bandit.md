# Level 0
ssh bandit0@bandit.labs.overthewire.org -p 2220

# Level 0 -> 1
ls
cat readme
ssh bandit1@bandit.labs.overthewire.org -p 2220

# Level 1 -> 2
ls
cat ./-

# Level 2 -> 3
ls
cat "spaces in this filename

# Level 3 -> 4
ls
cd inhere
ls -a
cat .hidden

# Level 4 -> 5
ls
cd inhere
file *
file ./*
cat ./-file07

# Level 5 -> 6
ls
cd inhere
ls
ls -al * | grep -B 10 1033
cat maybehere07/.file2

# Level 6 -> 7
cd ../..
find ./ -group bandit6 -user bandit7 -size 33c
found  ./var/lib/dpkg/info/bandit7.password
cat ./var/lib/dpkg/info/bandit7.password

# Level 7 -> 8
cat data.txt | grep millionth

# Level 8 -> 9
ls
sort data.txt | uniq -u

# Level 9 -> 10
ls
cat data.txt | grep "="
strings data.txt

# Level 10 -> 11
ls
cat data.txt
base64 -d data.txt

# Level 11 -> 12
ls
cat data.txt
used CyberChef cipher to decode ROT13
https://gchq.github.io/CyberChef/#recipe=ROT13(true,true,false,13)

# Level 12 -> 13 
ls
cat data.txt
mkdir /tmp/newfile666
cp data.txt /tmp/new123
cd /tmp/newfile666
xxd -r data.txt data
file data
mv data data.gz
gzip -d data.gz
file data
mv data data.bz2
bzip2 -d data.bz2
file data
mv data data.gz
gzip -d data.gz
file data
tar -x -f data
file data5.bin
tar -x -f data5.bin
file data6.bin
bzip2 -d data6.bin
file data6.bin.out
tar -x -f data6.bin.out
file data8.bin
mv data8.bin data8.gz
gzip -d data8.gz
file data8
cat data
















