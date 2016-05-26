# Assignment-8.4
Chapter 8 Lists
fname = raw_input("Enter file name: ")
fh = open(fname)
lst = list()
for line in fh:
    line = line.rstrip()
    words = line.split()
    for element in words:
        if element in lst:
            continue
        else:
            lst.append(element)
lst.sort()
print lst
