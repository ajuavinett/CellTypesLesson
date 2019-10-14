##  Accessing the Allen SDK
We could spend all day going through the cells in the website database to find some interesting comparisons. But, it’s much quicker to do these comparisons by accessing the entire database directly, through the Allen Software Development Kit (SDK).

If you're at UC San Diego, you can run this code on the UCSD Data Hub. Otherwise, you can run it locally on your computer.

#### Option 1: From the UCSD Data Hub
1. While either on campus or connected via VPN, go to <a href="http://datahub.ucsd.edu">http://datahub.ucsd.edu</a> and log in.

2. You’ll land on a page where you’re asked to choose a container to spawn. Choose the container with your course name.

3. On the Jupyter home page, go to New > Terminal (upper right corner).

4. Type  `git clone http://www.github.com/ajuavinett/CellTypesLesson.git`
to clone the necessary codebase into your folder.

5. Close the Terminal window. On the Jupyter dashboard, you should now see a folder CellTypesLesson. Click into it, and open “Introduction to Jupyter Notebooks” From here, you can follow the directions in the Jupyter Notebook. Au revoir!
* <b>Note</b>: When you’re done, go to the Running tab and Shutdown all of your terminal & notebook processes.

#### Option 2: From a local computer
If you’d like to access the SDK locally, follow these steps. 
<u>Note</u>: If you’re in BIPN145, you should do this lab through the Data Hub (Option 1 above).

1. Make sure that you have the <a href="https://www.anaconda.com/download/">Anaconda Python 3.7</a> distribution installed on your computer.
2. If necessary, <a href="https://git-scm.com/download/win">install Git</a> on your computer. You can click “Next” through all of the options.
3. If you're using Windows. Open an Anaconda Prompt window. This will open a new Python terminal. If you're using a Mac, simply open a Terminal window.
* Hint: Search for “Anaconda” in Windows and you should see come up as an option. Similarly, you can search for Terminal in Mac.
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
11. After the AllenSDK package has installed, you can open Jupyter Notebook in two ways:
* In Terminal,  type `jupyter notebook`
* Open the Anaconda Navigator, and click on Jupyter Notebook.
12. A Jupyter Notebook landing page (the Dashboard) should open.
13. On the dashboard, you should now see a folder CellTypesLesson. Click into it, and open “Introduction to Jupyter Notebooks” From here, you can follow the directions in the Jupyter Notebook. Au revoir!

### <a href="https://ajuavinett.github.io/CellTypesLesson/">Back to the start page</a>
