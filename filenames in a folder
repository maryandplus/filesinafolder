#python script for creating list of filenames
#number of the files is shown in the beginning of the text file

from os import listdir

mypath= r'xxxXXXxxx'

mydataset=[]

for file in os.listdir(mypath):
    if file.endswith(".img"):
        
        for i in range(len(os.listdir(mypath))):
            mydataset.append(os.path.join(mypath, file))
            break

#write filenames in a text file         
for j in range(len(mydataset)):
    print(mydataset[j])
    
    with open("mydataset.txt", "a") as myfile:
        newlines_mydataset=mydataset[j] + '\n'
        myfile.write(newlines_mydataset)

#write number of files
with open('mydataset.txt', 'r') as original: data = original.read()
with open('mydataset.txt', 'w') as modified: modified.write(str(len(mydataset))+'\n' + data)
