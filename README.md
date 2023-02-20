# tic-tac-toe
tic-tac-toe
#!/usr/bin/env python
import os 

# Get the current working directory 
cwd = os.getcwd() 
  
# List all the files in the current directory 
files = os.listdir(cwd) 
  
# Iterate over all the files in the current directory 
for file in files: 

    # Get the full path of each file in the current directory 
    full_path = os.path.join(cwd, file) 

    # Check if it is a file or a directory and print accordingly 
    if os.path.isdir(full_path): 
        print("Directory:", full_path) 

    else: 
        print("File:", full_path)
