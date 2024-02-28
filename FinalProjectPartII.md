See [Final Project Part I](FinalProjectPartI.md) and [Final Project Part III](FinalProjectPartIII.md)

# Wireframes / storyboards

I started building out a draft of my final project in ArcGIS StoryMaps. You can see the draft here: [TheNewCancerAlley](https://storymaps.arcgis.com/stories/cf5ab476dca242cd871dc464aaba0f40)

### Spatial Data

I started with the data. First, I downloaded a shapefile from the Pennsylvania Department of Environmental Protection (PA-DEP) showing oil and gas drilling sites across the state. In ArcGIS Pro, I created new layers showing only unconventional (fracking) wells, and restricted the geographic area to the 10-county region of Southwest PA. I made some stylistic changes, such as making the point features orange and the background black.

Then, I exported these layers as a new feature and created a time series. This way, the viewer can see the rapid growth of fracking development in the region since 2002. The time series was tricky-- it took a few hours of messing to get it to work the way I wanted.

### Set-up

Next, I drafted the set-up to this data after doing some basic research on the history of fracking. The most difficult part of the background section was finding open-source images. I used a combination of OpenVerse, Wikimedia Commons and Pexels to find my images. They're not perfect-- so I might change them in my final version.

Update 2/22: After consulting Sarah Young, I've learned that it's better not to include screenshots of news articles because some sites have copyright laws that would prevent this content from being copied. In my final draft, I'll make sure to remove the screenshots.

### Conflict
Next, I narrowed my focus to Southwest PA. I wanted to make this part of the story as personal as possible. Before grad school, I was working as an organizer for PennEnvironment, an environmental advocacy nonprofit. I spoke on the phone with a man who told me about his own experience living near fracking-- including what happened to his son. It turned out that he was involved in a lawsuit against the company and had been interviewed multiple times. I kept him anonymous in my story since I didn't get his permission to retell it. All of the details I included were also provided in public news stories that I was able to find online.

I felt like the map I included adequately showed the number of fracking wells in SWPA, but I also wanted to show how often fracking companies have been violating the law. There's a perception that as time goes on and technology supposedly advances, companies are doing a better job of following regulations and keeping pollution out of our environment. However, that's clearly not the case.

### Challenges

I have been struggling to build the visualization in Tableau. I downloaded an excel table from the Pa-DEP of all oil and gas violations in PA, and filtered to include only unconventional wells and SWPA counties. I then uploaded both this table and the spatial data on # wells to Tableau, and united these using a unique Site ID column. I used Spud Date (the date of drilling) for the column, and count of wells by spud date. I also added a calculation that counts the number of violations (using a field for a unique violation ID). However, the line it produced is not correct (it ultimately counts 7,000 some violations instead of 4,000 some). The calculation I used was Count([ViolationID]) and I set it to be a running total across spud date.

Update 2/22: After many hours I finally succeeded in making the Tableau graph! It just took a little more data cleaning in excel. I created new sheets and new columns with a function that takes only the month and year of Spud_Date and Violation_Date respectively. Then, I created a pivot table in each worksheet to show the count of wells or violations in each month/year combination. That way, I was able to match the two sheets based on month/year and display the running total of both well count and violation count based on month/year. I am relieved! 

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
- Were there any times that the language was difficult to understand or you noticed use of jargon?
- What did you want to know more about after viewing?

>See if the message of my story is working as intended
- What is the main message you take away from this story?
- Did you learn anything and/or change your opinions after viewing?	

>See if there are gaps in the evidence I provided or places to cut/expand on content
- Are you convinced that the story being told is correct? Did you feel there were any moments where I didn't provide enough evidence to back my claims?
- What are you still confused about? (Either about the substance or from the data visualizations)
- What, if anything, felt repetitive or irrelevant?

>Get suggestions for improved readability, aesthetics, and clarity
- How visually appealing was this story? Did you find your eye pulled in many directions? Did you feel like the theme matched the tone of the story?
- Any other feedback or changes you'd suggest?

		
## Interview findings
So far, I've heard back from one out of my three interviewees-- so there will be more feedback to come! Here's what they said:

**1. What is the main message you take away from this story?**		

Growing evidence suggests that fracking poses serious risks to our health and environment.	

**2. Did you learn anything and/or change your opinions after viewing?**

I learned that effects of fracking are far more serious to living things and the environment than I originally thought. The impacts are clearly connected to the introduction of fracking in an area, yet fracking continues to happen to due to other fiscal priorities.			

**3. Are you convinced that the story being told is correct? Did you feel there were any moments where I didn't provide enough evidence to back my claims?**		

I wanted more defintiive, big text, telling me the thesis of each section. For example, the first section describes the beginning of racking and the impacts of global warming, but I wanted one big quote at the end of that section outlining that "Later research would show that fracking produces about the same amount of global warming pollution as coal... if not more." That text was a little hidden in the paragraphs. Similarly, I wanted more clear connection between fracking wells in an area and the way that it impacted the people and environment (e.g., Why is the water in that one picture red? Why did the boy develop sores in the bath? Etc.)	

**4. What are you still confused about? (Either about the substance or from the data visualizations)**		

The interactive map of the US was cool (earlier in the presentation), but I wish my attention was directed to a specific part of the map. The blurb next to the map mentions levels spiked in 2005, but it's hard to navigate the map to see this spike without instruction.		

**5. Were there any times that the language was difficult to understand or you noticed use of jargon?**	

What is Ewing Sarcoma? What is lymphoma? What "kind" of cancer is it? Do people die from it		

**6. What did you want to know more about after viewing?**		
See question 3			

**7. What, if anything, felt repetitive or irrelevant?**	
n/a		

**8. Any other feedback or changes you'd suggest?**	

The news stories graphic is very powerful. I might feature each headline by itself for a few seconds as the reader scrolls so the headlines become more readable and dramatic. Is there a way to make each news article clip appear in succession rather than all at once?		
		
# Identified changes for Part III
I still need to hear feedback from my other two contacts, but for now, I'm planning on implementing most of the changes suggested by the first interviewee. Here's an outline of my plan:

-big text displaying thesis of each section

-see if I can embed the first map to the line graph instead of the map, since I reference the graph

-build out the story of the man in WA county a bit further to make the connection with fracking clearer, since not everyone will listen to the audio clip

-add more info on the seriousness of ewing sarcome and lymphoma

-Change the news articles clip: I have concerns about copyright on this anyways (perhaps make this part text headlines instead?)
