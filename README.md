# IWSLT-BACKUP
The link the IWSLT dataset link doesn't work anymore on torchtext, and even the updated link only works on the experimental dataset (Nightly version) which has a different API for loading the dataset. All of my code broke since I can't reproduce it.

To remedy this I uploaded the dataset it its old version in a way that supports the old API. You won't have to change your code, you should only place the dataset in your `.data` folder, or your root folder.

If anyone has a better solution hit me up please.

## Quick guide

Run these commands in the same folder as your script. 

     #Download the repo
     wget https://github.com/maroxtn/IWSLT-BACKUP/archive/main.zip -q

     #Extract the zip
     unzip -q main.zip

     #Move the dataset under .data/ directory
     mkdir .data
     mv IWSLT-BACKUP-main/iwslt .data

     #Delete unnecessary files
     rm -rf main.zip IWSLT-BACKUP-main

Then you can simply load the dataset using torchtext same as before, an example is provided in the `Test notebook.ipynb` notebook.

Hope you find this useful.