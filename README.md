# 3D MRI Dataset Classification and Interpretation Study

## Part 1: Data Download

### Step 1: Accessing the Dataset
- Navigate to the Alzheimer's Disease Neuroimaging Initiative (ADNI) database at the following URL: [ADNI Data Repository](https://ida.loni.usc.edu/home/projectPage.jsp?project=ADNI).
- Click on the 'Download' button on the menu bar and select 'Image Collections'.

### Step 2: Filtering the Dataset
- In the menu, select 'Advanced Search'.
- Under 'Search Options – Image Types', select 'Original'.
- For 'PROJECT/PHASE - PHASE', choose 'ADNI 3'.
- Within 'SUBJECT-Research Group', select 'MCI', 'AD', 'CN'.
- Under 'IMAGE-Modality', choose 'MRI'.
- In the 'IMAGING PROTOCOL - Matrix Z', select 'Equals 176'.
- For 'IMAGING PROTOCOL - Acquisition Type', choose '3D'.
- Choose 'T1' for 'IMAGING PROTOCOL - Weighting'.
- Click 'Search'.

### Step 3: Downloading the Images
- In the 'Advanced Search Results', check 'select all' and then choose 'add to collection'.
- Create your own collection and name it.
- You will be redirected to your collection, where you should check 'ALL' and click '1-click download' to complete the image download process.

#### Additional Step: Downloading Label Information
- Click on 'csv' to download the corresponding label information.
- Note: We need only the data described as 'Accelerated Sagittal MPRAGE'. 'Accelerated Sagittal MPRAGE_ND are not needed'
- The data will now be saved locally on your computer.

## Part 2: Data Preprocessing
- Use the provided Preprocess.ipynb for this step
- Download 'conform.py' file before running the previous code. Change the directory as needed.

## Part 3: FastSurferCNN for whole brain segementation

- Visit the github for building the environment  https://github.com/Deep-MI/FastSurfer/tree/stable
- Follow their colab tutorial for the segementation. You could also do the job on colab. 
https://github.com/Deep-MI/FastSurfer/blob/stable/Tutorial/Tutorial_FastSurferCNN_QuickSeg.ipynb

## Part 4: Model Training

- Utilize the code provided in this GitHub link to train the model. Please make appropriate adjustments to accommodate the local storage method.
