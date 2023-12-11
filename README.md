# DSC180A_Q1
This is the code and data I used to create my predictive models for my quarter 1 final project. All necessary files are located in the main branch.

Reproducing the project:
Step 1: Acquiring Data
-The first thing you will need to do is to clone this repository to your local device and then download/unzip the files. There are 4 datasets I used and they are called, train.tsv (in the Liar_plus folder), equal_random_sample_df.csv.zip, equal_random_sample_processed.csv, and politifact_data_combined_prev_ratings.csv.zip. Once those are unzipped, I would put them all back in a folder called Data, and put the Liar_plus folder with train.tsv in it in the Data folder as well. This will allow for no changes needed to be made in the ipynb file I have provided.

Step 2: Creating DSC180A_Q1 environment
-The next step is to create the conda environment with all the necessary dependencies to run the ipynb file I've provided. To do this you will need to open up your terminal on your local device. Make sure you have also downloaded the environment.yml file to your local device as well. You will navigate to where your environment.yml is in the terminal and then run the following line of code.
- conda env create -f environment.yml
-This will create a conda environment for you where you will have all the necessary dependencies. From here, you can open a jupyter notebook or whatever environment you usually program in and open the LiarLiarTesting.ipynb file provided.

 Step 3: Running LiarLiarTesting.ipynb
 -Running the LiarLiarTesting.ipynb should be fairly straightforward but there are a couple things to keep in mind. Firstly, if for any reason a package wasn't properly downloaded you can do a simple google search to find the pip installation and it should work with the latest versions of all packages as of December 11th, 2023. Once this is done we can get to the rest of the code.
 -All you need to do is run the code line by line to reproduce the results I obtained. The only hiccup is once you reach the section called "Using Perigon News API to Enrich Data." In this section you will notice that the second code block is commented out and reads 
 #COMMENT THE FOLLOWING LINE BACK IN IF YOU HAVE YOUR OWN ACCESS TO PERIGON NEWS API REQUESTS. THIS WILL ALLOW YOU TO CREATE YOUR OWN SUBSET OF THE DATA TO TRAIN AND TEST ON
 -This is because the PERIGON NEWS API has limited access and you are only permitted 500 news API requests with the version I obtained through contacting them. This means that reproduction is very difficult, so instead I provided the datasets I used with the news API prior to obtaining the data, as well as after the processing and tokenization of the data. If you run the third cell you will see the dataset I used before processing it. You will then see another code block that reads,
### ONLY RUN THE NEXT 7 CELLS IF YOU HAVE YOUR OWN PERIGON API KEY AND RESOURCES
-You should skip the next 7 code blocks if you dont have your own PERIGON API Key and account. After the next 7 code blocks there is a cell that reads,
### START AGAIN AT THIS CELL IF NOT USING YOUR OWN PERIGON API DATA
-You should begin again here and the next code block loads back in the processed dataset I obtained from the 7 code blocks above. If you continue from here you should get all the same results that I obtained. This concludes everything you need to do to reproduce this project. Thank you.

