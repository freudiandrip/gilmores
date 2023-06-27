# LEDE PROJECT 1 ANALYSIS
### The Gilmore Girls Literary Canon
Completed project can be found [here]("nguyenkim.ca/data-viz/gg/gilmores")

## 1. Project Motivations
This project was an excuse to apply some D3 using a dataset with nice sample size in the hundreds. Even though book data isn't as accessible as previously (RIP Goodreads), it's still readily available and relatively easy to obtain if you're willing to poke around. 

Technical aspects aside, the subject matter is interesting to me (books), and I thought it would be stylistically fun to apply it to Gilmore Girls, a show about books.

## 2. Findings 
The project's hypothesis posits what type of books do the Gilmores read, and how does the practice of reading play into the broader culture they exist in?
 
By parsing through the series' literary canon, we have a rich amount of data that quantifies the Gilmores' reading habits in a qualitative context.

### 2.1 Preliminary design choices
After obtaining the data, I was primarily interested in using D3 to visualize it because I had a vision of how the chart looked and only D3 allowed for the fine-tuning that was needed to bring it about.

Because the graphic was measured one-dimensionally, I decided on using a beeswarm plot. Beeswarm plots aren't available on data wrapper / flourish or you needed to pay in order to use it, confirming my choice in using D3.

### 2.2 The shape of the data
From the data, it turns out the characters in the Gilmore-verse are pretty much game for anything but generally stick to titles released in the 20th and 21st centuries. 

Initially, I employed both an exponential and linear scale to plot out the titles, but because the data was so heavily skewed towards more modern titles, the linear scale was breaking on the update transition which lead me to abandoning it and sticking with just a single scale. 


## 3. Methodology
#### Design stack:
- Figma
- Adobe Photoshop

#### Tools used:
- Scraping + Processing (Python): 
	- Wiki API
	- OpenLib Books and Covers API
	- GRScraper
	- Jupyter Lab + Pandas
- Visualization (JS):
	- D3

### 3.1 Collection
The following methods were used in order to obtain the data
- Obtaining a .csv export of a goodreads list to export to OPENLIB
- Using OPENLIB's Api 
- Concurrent Scraping 

### 3.2 Analysis

## 4. Reflections
As with any project that involves data, collecting it then analyzing took up the bulk of my time. 90% was devoted to data (collecting, parsing + cleaning, visualizing), with the remaining 10% spent on design, laying out the page, writing, design.

## 5. Next Steps
Addressing the issues + nice to haves in 5.1 and 5.2 would basically make this a perfect project.

### 5.1 Issues to fix
- Inconsistencies in language and UTF formatting (titles are in Cyrillic, Greek, etc.); get it all in English and UTF-8
- Inconsistent formatting and gaps in data from user input (or lack of it).
- Infobox responsiveness with a `@media` query + flex.
- Refine genres and subjects per title.
- Cross validate with different sources for incorrect year info based on edition or bad user input (which will skew the data).

### 5.2 Things to **zhuzh** the project
- Another graphic
- D3 annotations would make the chart really pretty.
- Create filters based on genre or subject matter.
- Allow users to slice / zoom into certain periods for deeper analysis.
- Add some nicer JS animations in the page.
- Expand on the hypothesis a bit more to make it a fully fleshed out written piece.
-----------------------------
contact: hi@nguyenkim.ca