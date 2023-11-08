# 3D MRI Dataset Classification and Interpretation Study

## Part 1: Data Download

### Step 1: Accessing the Dataset
- Navigate to the Alzheimer's Disease Neuroimaging Initiative (ADNI) database at the following URL: [ADNI Data Repository](https://ida.loni.usc.edu/home/projectPage.jsp?project=ADNI).
- Click on the 'Download' button on the menu bar and select 'Image Collections'.

### Step 2: Filtering the Dataset
- In the menu, select 'Advanced Search'.
- Under 'Search Options – Image Types', select 'Original'.
- For 'PROJECT/PHASE - PHASE', choose 'ADNI 1'.
- Within 'SUBJECT-Research Group', select 'MCI', 'AD', 'CN'.
- Under 'IMAGE-Modality', choose 'MRI'.
- In the 'IMAGING PROTOCOL - Matrix Z', select 'Equals 160'.
- For 'IMAGING PROTOCOL - Acquisition Type', choose '3D'.
- Choose 'T1' for 'IMAGING PROTOCOL - Weighting'.
- Click 'Search'.

### Step 3: Downloading the Images
- In the 'Advanced Search Results', check 'select all' and then choose 'add to collection'.
- Create your own collection and name it.
- You will be redirected to your collection, where you should check 'ALL' and click '1-click download' to complete the image download process.

#### Additional Step: Downloading Label Information
- Click on 'csv' to download the corresponding label information.
- Note: We need only the data described as 'MPRAGE'. Approximately half of the data does not fit this description, and currently, there is no refined method to select this subset of data more specifically.
- The data will now be saved locally on your computer.

## Part 2: Data Preprocessing

- Use the 'conform.py' file provided in the compressed package to preprocess each '.nii' file. This will generate segmented '.nii' files ready for training.

## Part 3: FastSurferCNN for whole brain segementation

- Visit the github for building the environment  https://github.com/Deep-MI/FastSurfer/tree/stable
- Follow their colab tutorial for the segementation. You could also do the job on colab. 
https://github.com/Deep-MI/FastSurfer/blob/stable/Tutorial/Tutorial_FastSurferCNN_QuickSeg.ipynb

## Part 3: Model Training

- Utilize the code provided in this GitHub link to train the model. Please make appropriate adjustments to accommodate the local storage method.
