# INeuron-ML-Assignment-Exception-Handling

#Exception handling
while True:
    try:
        d = int(input("input a denominator d for 5/d="))
        r= 5/d
        print("Result of 5/d is:", r)
        break
    except Exception as e:
        print("Your input value is incorrect.", e)
        continue
        
#Generate sentences
#Implement a Python program to generate all sentences where subject is in
#["Americans", "Indians"] and verb is in ["Play", "watch"] and the object is in
#["Baseball","cricket"].

#Initializing lists
subjects=["Americans","Indians"]
verbs=["play","watch"]
objects=["Baseball","Cricket"]
list=[]

try:
    def gen_phrase(subjects, verbs, objects):
        for sub in range(len(subjects)):
               for verb in range(len(verbs)):
                    for obj in range(len(objects)):
                          list.append(subjects[sub]+" "+ verbs[verb]+" "+objects[obj])
                    
    
except Exception as e:
    print(e)
   
    

gen_phrase(subjects, verbs, objects)
for i in range(len(list)):
    print(list[i])
