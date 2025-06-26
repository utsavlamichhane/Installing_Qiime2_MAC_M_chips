# Step 1

Open a new terminal in your mac

# Step 2

Create a new directory using the following command:

```
mkdir -p ~/miniconda3
```

# Step 3

Then get the .sh (script) using the following code:

```
curl https://repo.anaconda.com/miniconda/Miniconda3-latest-MacOSX-arm64.sh -o ~/miniconda3/miniconda.sh
```

Then run the following code:

```
bash ~/miniconda3/miniconda.sh -b -u -p ~/miniconda3
```

# Step 4

Remove the above .sh file after running hte codes. Run the following code in the terminal:

```
rm ~/miniconda3/miniconda.sh
```

# Step 5

Close and quit the terminal.

# Step 6

Open a terminal again.

# Step 7

Lets intitalize the conda by running following two codes in sequence:

```
source ~/miniconda3/bin/activate
```

```
conda init --all
```

# Step 8

Close the terminal and quit it. 
