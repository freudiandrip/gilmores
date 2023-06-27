# LEDE PROJECT 1 ANALYSIS
### The Gilmore Girls Literary Canon
Completed project can be found [here]("https://nguyenkim.ca/data-viz/gg/gilmores")

## 1. Project Motivations
This project was an excuse to use D3 using a dataset with nice sample size in the hundreds. Though book data isn't as accessible as previously (:headstone: Goodreads), it's still relatively easy to obtain. 

Technical aspects aside, the subject matter is interesting to me, and I thought it would be stylistically fun to apply it to Gilmore Girls, a show about books.

## 2. Findings 

### 2.1 Preliminary design choices
After obtaining the data, I was primarily interested in using D3 for fine-tuning.

Because the graphic was measured one-dimensionally, I decided on a beeswarm plot. Beeswarm plots aren't available on data wrapper / flourish or require a premium subscription, confirming my choice in using D3.

### 2.2 The shape of the data

The data followed an exponential pattern (with the bulk landing in the 1900s-2000s+), warranting an exponential scale for linearization.

Initially, both an exponential and linear scale were used to plot out the titles but the data was so heavily skewed, the linear scale was breaking on update which lead to scaling the data exponentially.

## 3. Methodology
#### Design stack:
- Figma
- Adobe Photoshop

#### Tools used:
- Scraping + Processing + Viz: 
	- Wiki API
	- GRScraper
 	- OpenLib Books and Covers API
	- Jupyter Lab + Pandas
	- D3

### 3.1 Collection
The following methods were used in order to obtain the data
- Obtaining a .csv export of a goodreads list to export to OPENLIB
- Using OPENLIB's Api 
- Concurrent Scraping
- Compile data, prepped for analysis 

### 3.2 Analysis
- Pandas processing + cleaning
- Output to CSV, feed into JS + D3 (processing on the fly + viz)

## 4. Reflections
Collecting data then analysis made up the bulk of work. 90% was devoted to data (collecting, parsing + cleaning, visualizing), with the remaining 10% spent on design, laying out the page, writing, design.

## 5. Next Steps
Addressing the issues + nice to haves in 5.1 and 5.2

### 5.1 Issues to fix
- Inconsistencies in language and UTF formatting (titles are in Cyrillic, Greek, etc.); English and UTF-8
- Inconsistent formatting and gaps in data from user input (or lack of it).
- Infobox responsiveness with a `@media` query + flex.
- Refine genres and subjects per title.
- Cross validate for incorrect year info based on edition or faulty user input.

### 5.2 Nice to haves
- Another graphic
- D3 annotations 
- Create filters based on genre or subject matter.
- Allow users to slice / zoom into different periods.
- JS animations
- Expand to make it a fully fleshed out written piece.
-----------------------------
contact: hi@nguyenkim.ca
