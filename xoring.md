xoring <br>
xored is given in ascii <br>
and we need to find the flag by solving it<br>
our flag starts with wired <br>
we need to find wired in xored by converting ascii to character <br>
for that we need to assigne secret = "wired "**xored <br>
wired in " " because we need to find wired in the ascii list (xored)<br>
we use chr(ord(a) ^ ord(b) because we need to change the elements in the list xoring from ascii to character 
