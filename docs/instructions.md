# Accessing the Allen Cell Types Dataset on their website

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




### <a href="https://ajuavinett.github.io/CellTypesLesson/">Back to the start page</a>
### <a href="https://ajuavinett.github.io/CellTypesLesson/computing">To the next step (Computing Basics)</a>
