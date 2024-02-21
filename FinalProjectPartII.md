# Wireframes / storyboards

I started building out a draft of my final project in ArcGIS StoryMaps. You can see the draft here: [TheNewCancerAlley](https://storymaps.arcgis.com/stories/cf5ab476dca242cd871dc464aaba0f40)

### Spatial Data

I started with the data. First, I downloaded a shapefile from the Pennsylvania Department of Environmental Protection showing oil and gas drilling sites across the state. In ArcGIS Pro, I created new layers showing only unconventional (fracking) wells, and restricting the geographic area to the 10-county region of Southwestern PA. I made some stylistic changes, such as making the point features orange and the background black.

Then, I exported these layers as a new feature and created a time series. This way, the viewer can see the rapid growth of fracking development in the region since 2002.

### Set-up

Next, I drafted the set-up to this data after doing some basic research on the history of fracking. The most difficult part of that was finding open-source images. I used a combination of OpenVerse, Wikimedia Commons and Pexels to find my images. They're not perfect-- so I might change them in my final version.

### Conflict
Then, I narrowed my focus to Southwest PA. I wanted to make this part of the story as personal as possible. Before grad school, I was working as an organizer for PennEnvironment, an environmental advocacy nonprofit. I spoke on the phone with a man who told me about his own experience living near fracking-- including what happened to his son. It turned out that he was involved in a lawsuit against the company and had been interviewed multiple times. I kept him anonymous in my story since I didn't get his permission to retell it. All of the details I included were also provided in public news stories that I was able to find online.

I felt like the map I included adequately showed the number of fracking wells in SWPA, but I also wanted to show how often fracking companies have been violating the law. There's a perception that as time goes on and technology supposedly advances, companies are doing a better job of following regulations and keeping pollution out of our environment. However, that's clearly not the case.

###Challenges

I have been struggling to build the visualization in Tableau. I downloaded an excel table from the Pa-DEP of all oil and gas violations in PA, and filtered to include only unconventional wells and SWPA counties. I then uploaded both this table and the spatial data on # wells to Tableau, and united these using a unique Site ID column. I used Spud Date (the date of drilling) for the column, and count of wells by spud date. I also added a calculation that counts the number of violations (using a field for a unique violation ID). However, the line it produced is not correct (it ultimately counts 7,000 some violations instead of 4,000 some). The calculation I used was Count([ViolationID]) and I set it to be a running total across spud date.

### Resolution and Call to Action
I moved on from this data visualization to focus on the rest of the story. Beyond plenty of literature and news stories, I haven't found much raw data on health impacts (this type of public health data is, apparently, notoriously difficult to find). But I am considering exploring other data on methane pollution and, possibly, cancer rates. (I am concerned that showing spatial data on cancer rates would be misleading without a comprehensive analysis on whether fracking is a factor, since higher cancer rates in SWPA could be due to many other factors too).

Finally, I developed some policy recommendations based on the Grand Jury report and the recommendations of advocacy groups.

# User research

## Target audience

I want to reach a somewhat broad audience with my story (it probably won't reach the average person, but it might reach people interested in policy or environmental health who aren't professionals in these fields), so I selected three individuals with varying levels of expertise and age. 
> The first is a young professional with policy expertise (but not in the field of environmental policy) and data visualization experience.
> The second is a middle-aged psychologist with no professional policy expertise.
> The third has expertise in environmental policy and advocacy, including fracking.

## Interview script

My goals for this research are to:

>Find out how easily understood my story and visualizations are

>See if the message of my story is working as intended

>See if there are gaps in the evidence I provided or places to cut/expand on content

>Get suggestions for improved readability, aesthetics, and clarity

The questions I asked were:

1. What is the main message you take away from this story?			
2. Did you learn anything and/or change your opinions after viewing?	
3. Are you convinced that the story being told is correct? Did you feel there were any moments where I didn't provide enough evidence to back my claims?	
4. What are you still confused about? (Either about the substance or from the data visualizations)
5. Were there any times that the language was difficult to understand or you noticed use of jargon?
6. What did you want to know more about after viewing?	
7. What, if anything, felt repetitive or irrelevant?	
8. How visually appealing was this story? Did you find your eye pulled in many directions? Did you feel like the theme matched the tone of the story?		
9. Any other feedback or changes you'd suggest?		
		
## Interview findings

| Questions               | Interview 1 (briefly describe) | Interview 2 | Interview 3 |
|-------------------------|--------------------------------|-------------|-------------|
| Question you asked here | Insightful feedback            |             |             |
|                         |                                |             |             |
|                         |                                |             |             |


# Identified changes for Part III
> Document the changes you plan on implementing next week to address any issues identified.  

Text here!

| Research synthesis                       | Anticipated changes for Part III                                                |
|------------------------------------------|---------------------------------------------------------------------------------|
| Findings or observations from interviews | Describe what, if any changes you anticipate making to address the observation. |
|                                          |                                                                                 |
|                                          |                                                                                 |
|                                          |                                                                                 |
| ...add more rows as necessary            |                                                                                 |

> ...include any final thoughts you have here. 

Text here!

# Moodboards / personas
> If you did this optional part, include details here.  Otherwise remove this section

Text here!
