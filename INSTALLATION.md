
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

# Step 9

Open a new terminal.

# Step 10

Update your conda using the following code:

```
conda update conda
```

The terminal will ask you [y]/n. Type y and enter.

# Step 11

Close and quit the terminal. 

# Step 12

This is the first step in configuring the Terminal to use Rosetta

Open a new finder and open applications.

# Step 13

Find the Terminal inside the utilities.

# Step 14

Right click on the Terminal and select duplicate from the appearing options. 

After this, you will see another Terminal icon named Terminal copy.

For ease, rename that Terminal capy as Terminal_Rosetta

# Step 15

Now right click on this new Terminal_Rosetta and click in get info.

# Step 16

On the info tab, under the heading General you will see "Open using Rosetta".

Mark that box.

# Step 17

On the Terminal_Rosetta lets intall the QIIME2 version 2025.4

Run the following code in the Terminal_Rosetta:

```
CONDA_SUBDIR=osx-64 conda env create \
  --name qiime2-amplicon-2025.4 \
  --file https://raw.githubusercontent.com/qiime2/distributions/refs/heads/dev/2025.4/amplicon/released/qiime2-amplicon-macos-latest-conda.yml
conda activate qiime2-amplicon-2025.4
conda config --env --set subdir osx-64
```

 # THIS PROCESS WILL TAKE A WHILE


At the end, terminal might ask yes/no, go with  yes

# Step 18

Close and quit the Terminal_Rosetta


# Now you have QIIME2 Installed in your system

# step 19

Just to confirm that run the following command in your normal Terminal (no need to use the Terminal_Rosetta now onwards):

```
conda deactivate
conda activate qiime2-amplicon-2025.4
qiime info
```

If you see no error (red lines in your Terminal)

# Congratulations you have QIIME2 in your computer. 
