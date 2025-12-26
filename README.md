# Write-a-program-to-compute-the-number-of-characters-words-and-lines-in-a-file.
k = open('D:/a.txt', 'r')
char, wc, lc = 0, 0, 0
for line in k:
    lc += 1
    for i in range(0, len(line)):
        char += 1
        if line[i] == ' ':
            wc += 1
wc += lc
k.close()
print("The no.of chars is %d\nThe no.of words is %d\nThe no.of lines is %d"
      % (char, wc, lc))
