# Electrophysiological signatures of cell types in mouse & humans

## Table of contents

[Background](#background)<br/>
[Part I: Accessing the Allen Cell Types Dataset on their website](#part-i)<br/> 
[Part II. Accessing the Allen SDK](#part-ii)<br/>
[Data Notebook](#data-notebook)

## Background
In this lab, we’ll look at open-source data from mouse and human recordings in order to compare cell types from these creatures. We’ll dive into some of the different structures of dendrites, and how these might relate to the shape of their action potentials, and ultimately their role in neural computation.

<b>Before starting this lesson</b>, you should complete the <a href="https://www.codecademy.com/learn/learn-python-3">CodeAcademy tutorial for Python3 syntax</a>, or a similar tutorial that covers the basics of variables, `print ( )`, and arithmetic in Python.

### Learning objectives:
* Practice using Jupyter notebooks to run Python code and access the AllenSDK
* Understand the metrics that we can use to compare cell types
* Compare electrophysiological characteristics between humans and mice

### Part I.
#### Accessing the Allen Cell Types Dataset on their website
Before we go behind the scenes, we’ll look at a few cells on the Allen online interface to get a feel for what the data looks like.

1. Go to <a href="http://celltypes.brain-map.org/">http://celltypes.brain-map.org/</a>. Read through “About Electrophysiology” and “About Morphology” to answer questions 1 and 2 in the Data Notebook.

2. Scroll down to “Download Single Cell Data and Models” and the section “Morphology and Electrophysiology” and click on Electrophysiology Page. This page shows us all of the electrophysiology data for one sample cell that they have recorded from.

3. On the top, you’ll see a Mouse Line, Brain Area, and Layer where this cell comes from. Note them in Table 1.
The Mouse Line tells us the Cre-driver line that was used — in other words, the cells that they targeted had that gene, and therefore they also expressed Cre-recombinase. Go to <a href="https://www.ncbi.nlm.nih.gov/gene/">https://www.ncbi.nlm.nih.gov/gene/</a>and search for the name of this gene (without -Cre) to answer question 3.
This page also gives us some key details about the cell. Note the resting membrane potential in Table 1.

4. Click through the stimulus sweeps (the colored boxes) to find the first one that elicited an action potential.
Record the minimum stimulus amplitude required to elicit an action potential in this cell in Table 1.
<u>Note</u>: You should notice that this value is either very close or identical to the rheobase of the cell, as reported on the table on the top. As a reminder, the rheobase is defined as the minimum current needed to elicit an action potential. When the current is below the rheobase, an action potential will never occur regardless of how long the stimulation is.

5. Click through to a stimulus sweep with a higher current injection. Does the cell adapt to the stimulus? In other words, does the space between spikes increase? Is there a metric here that would help quantify this? Record that metric in Table 1.

6. Use the dropdown menu on the left to change the stimulus type to “Short square.” Record the minimum current needed to elicit an action potential at this stimulus, and answer question 4.

7. Use the dropdown menu on the left to change the stimulus type to “Noise.” Take a look at the current injection trace to get an idea of what this stimulus looks like. Note the differences between the cell’s response to this stimulus versus the square wave pulses. Answer question 5.

8. Click on View Morphology on the right, to check out the morphology of this cell. Take note of the distribution of the axon and the dendrites. Close this window.

9. Click on Cell Feature Search on the top right corner. Here, you can look through other cells in this dataset. Find a cell from human tissue that is in the same Layer and has the same Dendrite Type as the first cell you looked at. Use the data on that page to fill out Table 1.

###  Part II.
#### Accessing the Allen SDK
We could spend all day going through the cells in the website database to find some interesting comparisons. But, it’s much quicker to do these comparisons by accessing the entire database directly, through the Allen Software Development Kit (SDK).

If you're at UC San Diego, you can run this code on the UCSD Data Hub. Otherwise, you can run it locally on your computer.

#### Option 1: From the UCSD Data Hub
1. While either on campus or connected via VPN, go to <a href="http://datahub.ucsd.edu">http://datahub.ucsd.edu</a> and log in.

2. You’ll land on a page where you’re asked to choose a container to spawn. Choose the container with your course name.

3. On the Jupyter home page, go to New > Terminal (upper right corner).

4. Type  `git clone http://www.github.com/ajuavinett/CellTypesLesson.git`
to clone the necessary codebase into your folder.

5. Close the Terminal window. On the Jupyter dashboard, you should now see a folder BIPN 145. Click into it, and open “Introduction to Jupyter Notebooks” From here, you can follow the directions in the Jupyter Notebook. Au revoir!

6. When you’re done, go to the Running tab and Shutdown all of your terminal & notebook processes.

#### Option 2: From a local computer
If you’d like to access the SDK locally, follow these steps. 
<u>Note</u>: If you’re in BIPN145, you should do this lab through the Data Hub (Option 1 above).

1. Make sure that you have the Anaconda Python 3.7 distribution (https://www.anaconda.com/download/) installed on your computer.
2. Make sure that you have Git (https://git-scm.com/download/win) installed on your computer. You can click “Next” through all of the options.
3. Open an Anaconda Prompt window. This will open a new Python terminal.
* Hint: Search for “Anaconda” in Windows and you should see come up as an option.
4. Change directories into your Documents folder by typing `cd Documents`
5. Make a new folder for your Python notebooks by entering  `mkdir PythonNotebooks`
6. Check that your folder is there with the command dir. You should see PythonNotebooks in the list.
7. Move into your PythonNotebooks folder by using > cd PythonNotebooks
8. Next, we’ll clone the necessary Python notebooks into your Documents directory.
9. Type  `git clone http://www.github.com/ajuavinett/CellTypesLesson.git`
to clone the lab codebase into your folder.
10. Next, we need to install the allenSDK tools. Open a new Terminal window (if you’re in Windows, it needs to be an Anaconda terminal window) and type 
`pip install --user allenSDK`
<u>Note</u>: If you receive an error, try `pip install allenSDK`
11. After the allenSDK package has installed, you can open Jupyter Notebook in two ways:
* In Terminal,  type `jupyter notebook`
* Open the Anaconda Navigator, and click on Jupyter Notebook.
12. A Jupyter Notebook landing page (the Dashboard) should open.
13. On the dashboard, you should now see a folder BIPN 145. Click into it, and open “Introduction to Jupyter Notebooks” From here, you can follow the directions in the Jupyter Notebook. Au revoir!



### Data Notebook

1. Which method are the Allen researchers using to record from cells? _____________________________

2. What are the cells filled with to visualize their morphology? _________________________

3. Which neurotransmitter receptor does this gene code for? ______________________

4. Why would a longer stimulus require less current to elicit an action potential?

5. Why would you want to inject a noisy current into the cell?
(Not like 60 Hz noise, what we've been talking about before. "Noisy" current here is random, fluctuating around a certain value but not a perfect sine wave. To answer this question, consider what happens in a real neural circuit. Is the input as simple as a square wave?)


Table 1.

| Property | Mouse &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;                      | Human &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;                        |
|----------|:----------------------------:|:-------------------------------:|
| Cre Line || N/A |
| Area | | | 
| Layer | | |
| Dendrite type | | |
| Resting potential | | |
| Minimum current to elicit an AP with the long square wave | | |
| Minimum current to elicit an AP with a short square wave | | |
| Adaptation Index | | |





