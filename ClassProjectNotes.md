# Extend session for 5 days

(you will need to redo this 5 days later)

1. Log into jupyter.dartmouth.edu
2. Go through the typical steps of Starting/Stopping/Logging in/out to get it working
3. In the top right click New, Terminal
4. Type `rcdetach  sleep 5d` in terminal
5. Enter your netid and password when prompted
5. Close terminal window

# Transferring data to server

From your computer connect to the Psych 60 share link that we setup. If you are on a mac:

1. Click on your desktop, Go, Connect to server
2. smb://dartfs.dartmouth.edu/rc/lab/P/Psych60
3. Navigate to /students_output/YOURID
4. Copy your formatted onsets (.txt, tab delimited files, headers the same as the example .txt files in the project folder or from Lab_GLM.ipynb) to your output folder folder

# Running the class project

1. Open Class_Project_GLM_Template19W.ipynb
2. File, SaveAs, /Psych60/students_output/YOURID/Class_Project_GLM_YOURSTUDY19W.ipynb where your study is ScaryVSNotScary etc
3. Add your DID to the top of this file
4. Change results_dir to your output directory
5. Change path to onsets to something like: events1 = pd.read_csv(os.path.join("/dartfs/rc/lab/P/Psych60/students_output/","yourid","youronsetfileforrun1.txt"))
6. Do the same thing for events2
7. Change the conditions going forward, ie Dead, Alive to Scary, NotScary etc. There are multiple places you will have to do this.
8. If you are doing a 1-sample t-test you will need to change the subjects selected to the ones that you want. Please go through the QA files here and identify which subjects you want to include based on motion: https://jupyter.dartmouth.edu/user/d28603y/tree/Psych60/data/1001_Psych6019W/derivatives/fmriprep and clicking on each of the .html files
9. Same thing if you are doing a 2-sample t-test, say between individuals that were scared or not. The path to survey data is in the class template file.
