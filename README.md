file1=open('lower.txt','w')
file2=open('upper.txt','w')
file3=open('other.txt','w')
print("Press Enter to stop execution...")
while True:
    ch=input("Enter a character:")
    if ch=='':
        print("The contents of the files is shown below:")
        break
    elif ch.islower():
        file1.write(ch)
    elif ch.isupper():
        file2.write(ch)
    else:
        file3.write(ch)
file1.close()
file2.close()
file3.close()
print("\\'lower.txt\'")
file=open('lower.txt')
print(file.read())
print("\'upper.txt\'")
file=open('upper.txt')
print(file.read())
print("\'other.txt\"")
file=open('other.txt')
print(file.read())
file.close()
