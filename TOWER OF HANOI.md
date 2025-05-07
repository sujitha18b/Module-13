# Exp.No:13 E 
## TOWER OF HANOI



### AIM  
To write a Python program to implement **Tower of Hanoi** and display all the moves of the disks using a recursive function.  
Consider the names of the tower pegs as A, B, C. Get the number of disks value from the user.



### ALGORITHM  

1. **Start the program.**
2. **Input** the number of disks `n`.
3. **Print** the number of disks.
4. Define a **recursive function** `TowerOfHanoi(n, source, destination, auxiliary)`:
   - If `n == 1`:
     - Print: "Move disk from source to destination".
   - Else:
     - Call `TowerOfHanoi(n - 1, source, auxiliary, destination)`  
       → Move `n-1` disks from source to auxiliary using destination as helper.
     - Print: "Move disk from source to destination"  
       → Move the largest disk to the destination.
     - Call `TowerOfHanoi(n - 1, auxiliary, destination, source)`  
       → Move `n-1` disks from auxiliary to destination using source as helper.
5. Call `TowerOfHanoi(n, 'A', 'C', 'B')` to start the process.
6. **End the program.**



### PROGRAM  

def TowerOfHanoi(n , source, destination, auxiliary):  <br />
    if(n>0):  <br />
        TowerOfHanoi(n-1,source,auxiliary,destination) <br />
        print(f"Move disk from {source} to {destination}") <br />
  
n=int(input()) <br />
print("No. of disks =",n) 

### OUTPUT

![Screenshot 2025-05-07 105328](https://github.com/user-attachments/assets/a5cedace-582b-4a39-b0cc-ea61eefe0386)



### RESULT
 Thus, the given python program is implemented and executed sucessfully.
