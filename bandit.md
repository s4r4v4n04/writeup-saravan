# Level 0
ssh bandit0@bandit.labs.overthewire.org -p 2220

# Level 0 -> 1
ls<br>
cat readme<br>
ssh bandit1@bandit.labs.overthewire.org -p 2220<br>

# Level 1 -> 2
ls
cat ./-

# Level 2 -> 3
ls<br>
cat "spaces in this filename

# Level 3 -> 4
ls<br>
cd inhere<br>
ls -a<br>
cat .hidden<br>

# Level 4 -> 5
ls<br>
cd inhere<br>
file *<br>
file ./*<br>
cat ./-file07<br>

# Level 5 -> 6
ls<br>
cd inhere<br>
ls<br>
ls -al * | grep -B 10 1033<br>
cat maybehere07/.file2<br>

# Level 6 -> 7
cd ../..<br>
find ./ -group bandit6 -user bandit7 -size 33c<br>
found  ./var/lib/dpkg/info/bandit7.password<br>
cat ./var/lib/dpkg/info/bandit7.password<br>

# Level 7 -> 8
cat data.txt | grep millionth<br>

# Level 8 -> 9
ls<br>
sort data.txt | uniq -u<br>

# Level 9 -> 10
ls<br>
cat data.txt | grep "="<br>
strings data.txt<br>

# Level 10 -> 11
ls<br>
cat data.txt<br>
base64 -d data.txt<br>

# Level 11 -> 12
ls<br>
cat data.txt<br>
used CyberChef cipher to decode ROT13<br>
https://gchq.github.io/CyberChef/#recipe=ROT13(true,true,false,13)<br>

# Level 12 -> 13 
ls<br>
cat data.txt<br>
mkdir /tmp/newfile666<br>
cp data.txt /tmp/new123<br>
cd /tmp/newfile666<br>
xxd -r data.txt data<br>
file data<br>
mv data data.gz<br>
gzip -d data.gz<br>
file data<br>
mv data data.bz2<br>
bzip2 -d data.bz2<br>
file data<br>
mv data data.gz<br>
gzip -d data.gz<br>
file data<br>
tar -x -f data<br>
file data5.bin<br>
tar -x -f data5.bin<br>
file data6.bin<br>
bzip2 -d data6.bin<br>
file data6.bin.out<br>
tar -x -f data6.bin.out<br>
file data8.bin<br>
mv data8.bin data8.gz<br>
gzip -d data8.gz<br>
file data8<br>
cat data<br>
















