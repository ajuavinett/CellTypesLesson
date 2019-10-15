## Information about Allen Institute Cell Types Dataset
The dataset we'll be interacting with in this notebook was collected by the Allen Institute for Brain Science. I'd recommend watching this video so that you can see the people behind the data:

[![Allen Institute Video](http://img.youtube.com/vi/1GWyjxzxqII/0.jpg)](https://www.youtube.com/watch?v=1GWyjxzxqII "Allen Cell Types Database: Understanding the fundamental building blocks of the brain")

### Targeting different cell types
How did the Allen actually distinguish between different cell types? We can take advantage of the fact that different cells express different genes. With genetic engineering, we can express glowing proteins (such as green fluorescent protein) in cells that express a specific gene. This approach takes advantage of an enzyme called <b>Cre recombinase</b> that is found in bacteriophages, but not mammals. When we artifically express Cre recombinase in a specific cell type and use something called <b>LoxP</b> sites around our glowing protein, the Cre recombinase comes and flips those LoxP sites around, leading to protein expression and a gorgeous glowing neuron. This system is called the <b>Cre-LoxP</b> system and is one of the main tools that neuroscientists use to identify and target specific cells in the brain.

> You can find more about the Cre-LoxP system <a href="https://www.jax.org/news-and-insights/2006/may/the-cre-lox-and-flp-frt-systems">here.</a>

### Whole-cell patch clamp
In order to listen to neurons, the Allen researchers guided glass electrodes towards their glowing neurons under a microscope. Instead of poking into the cell to listen to it, they lowered the electrode very close the cell, and created a tiny bit of suction to break the cell membrane. As a result, the internal cell space becomes continuous with the electrode and enables really clean recordings of the cell's activity. This technique is called <b>whole-cell</b> patch clamp. It's a tough technique, but one that has proven irreplacable in our understanding of how cells communicate.

### Characterizing the electrophysiology of cells
You'll find many different metrics describing what happens when the Allen researchers stimulated and recorded from different cells. Let's breakdown what a few of these properties are actually measuring.

| Codename                | Full definition   
| -------------           |------------------------------------|
| vrest                   | resting membrane potential         |
| upstroke-downstroke     | ratio of action potential upstroke to downstroke |
| adaptation     | the rate at which firing speeds up or slows down during a stimulus |
| avg_isi        | the mean value of all interspike intervals in a sweep |
| trough_v_short_square | minimum value of the membrane potential during the after-hyperpolarization |

---

## Resources
* <a href="https://www.jax.org/news-and-insights/2006/may/the-cre-lox-and-flp-frt-systems">Jax Explanation of Cre-Lox systems</a>
* <a href="http://help.brain-map.org/download/attachments/8323525/CellTypes_Ephys_Overview.pdf">Allen Brain Institute Documentation</a>

## Sample publications with the Allen Cell Types dataset
Kalmbach et al. (2018) “<a href="https://www.cell.com/neuron/fulltext/S0896-6273(18)30900-0">h-Channels Contribute to Divergent Intrinsic Membrane Properties of Supragranular Pyramidal Neurons in Human versus Mouse Cerebral Cortex</a>”
“<a href="https://www.biorxiv.org/content/early/2018/07/17/368456">Classification of electrophysiological and morphological types in mouse visual cortex</a>” 
Hodge et al., 2018. “<a href="https://www.biorxiv.org/content/early/2018/08/05/384826">Conserved cell types with divergent features between human and mouse cortex</a>” 


## Navigation
### <a href="https://ajuavinett.github.io/CellTypesLesson/">Back to the start page</a>
### <a href="https://ajuavinett.github.io/CellTypesLesson/instructions">To the next step (Allen Website)</a>
