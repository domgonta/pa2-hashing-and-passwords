1. We have 2 hashes for the full password that is entered. Then we have 12 hashes for the letters that were inputed. 
"s" + "e" + "c" + "r" + "e" + "t" is 6, and there was 2 passwords with the same amount of letters, mkaing it 12. 
We then have three numbers at the end of the password input. For each digit, integers 0-9 are replaced except the 
original number to try every variation. Cause there is 3 numbers and 9 integers were tested, there would be 27 hashes. 
Because there are two passwords with the same amount of numbers, it would be 54 hashes. In total, 2 + 12 + 54, which 
would be 68 hases for testing.
2. For checking duplicates, we look at the passwords. The letters in the password are both secret, and each letter can 
be changed to capital letters. Because there are 6 letters, there are 6 duplicates that are hashed and checked. For the
integers, there are two duplicates, which are 1 and 1. To check for the integers, it has to go through 0-9, not counting
1 . Cause there are 9 integers to check and there are 2 duplicates, there would be 18 hashes for the integers. 6 + 18 = 
24 duplicates checked.
3. We could handle case and digit modifications separately. We can hash and generate only case modifications, and then
separately hash and generate only digit modifications. With having these work separately, it avoids repeated and redundant
work to ensure smooth and non overlapping ways. Another way I can chnage my implementation is already have all the 
possible outcomes for each character ready and hash each entry sepretely
