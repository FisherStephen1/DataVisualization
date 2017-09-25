<h2> Tableau </h2>

<h3>Tableau in a Computer Lab</h3>

**SetUp**
- student should first be registered at Tableau Public (not professional or educator version)
- if connecting to Tableau Public from a lab computer, student should make sure previous user has logged out
- open browser > public.tableau.com

**If Tableau is not previously installed**
- enter email address > download the app (10-0-1) > 30 seconds
- in download bar, find Tableau 10-0-1.dmg in Finder > double click
- Tableau verifies for 1 minute
- drag Tableau icon to Application folder > requires Authenticate
- Enter UserName Journalism Admin > wait for professor to enter password
- Tableau is copied to Applications for 1 minute
- Doubleclick Tableau Public in Applications > Tableau Desktop opens
- Students can look at Discover videos in right grey bar out of class

<h3>Tutorial</h3>
From NICAR 2014 Tableau Training Guide

Return to opening page: public.tableau.com
**Data**
- Under Resources in top grey bar, click Sample Data Sets
- Scroll to Lifestyle > Top Baby Names > click Dataset (csv versus xls files) > The file, TopBabyNamesbyState.csv, downloads
- double click csv file > enter first name for Office Mac, if required > Excel opens > double click csv file again
- inspect csv data: column names and 10507 rows! > (Occurrences spelled wrong) close Excel
- In Applications on the lab computers, find and open Tableau Public; in left blue column, Connect not to Excel but to a text file > double click TopBabyNamesbyState.csv
- inspect column headings and Tableau Public Symbols in column headings
- in lower left, click Sheet 1, beneath Go to Worksheet

**Worksheet**

Pause here to inspect Dimensions and Measures: Review Necessary Definitions:
- Measure: A variable from the dataset that is meant to be aggregated. This means it should be a number that it makes sense to do math with: sum, average, etc. In our dataset, the only Measure is “Occurrences” -- how many baby names. We would not do math with years, such as 2012 minus 1910. Years are not Measures.
- Dimension: A category variable from the dataset, often column headings, that we use to start understanding the data. State, year, gender, and name are all Dimensions in this dataset.
- Sheet: A sheet is a single work space in Tableau.
- Dashboard: A dashboard is a kind of canvas for displaying multiple sheets at a time. Ultimately you publish Dashboards.
- Workbook: A workbook is the entire Tableau file of your sheets and dashboards for a project.
- Filter: A filter is used to filter or limit what data is being displayed on the sheet. For example, you might look only at Gender and you might filter even more for Male or Female. You often want to Show Filter on a sheet or dashboard so viewers can interact.
- Pages: Pages are used to quickly flip between different views of a sheet. The most common use of pages is to show data for particular points in time.
- Legend: A legend, as with any chart, shows the meanings of color, size or objects.
- Tooltip: Tooltips are text boxes that appear when viewers hover over a mark on a sheet. They give more information and interactivity. The text and formatting in them are easily edited through the Marks card.
- Marks card: The marks card is the tool area, when creating a sheet, that controls most of the visual elements ("marks"). Using the marks card, you can switch between different chart types (bar chart or map, for example), change the colors, change sizes, add labels, change tooltips, change the level of detail and more.
- Rows and Columns Shelves: The rows shelf and the columns shelf is where you decide what variables will go on what axis. Put data you want displayed along the X‐axis on the columns shelf and data you want displayed on the Y‐axis on the rows shelf. These are easily changed and manipulated.

**Creating the Map**
- We are still at the open Tableau worksheet.
- Inspect where Tableau has put our variables. If Tableau had mistakenly put Years in Measures, it is easy to drag to Dimensions.
- Because we want to make a map, drag states to Marks > blue dots appear in each state
- Because we want to make a map with filled colors, not dots, click the drop down menu under Marks/Automatic, select Filled Map; the states are now filled with blue
- We want to start studying top names per state: drag Top Name to Color and drag Top Name again to Label (it is a big file but Add all members if asked) > the map now has names and colors in each state; a list of names also appears
- But we want to filter by names of boys and girls; drag gender to filters > in the popup box, choose M and F and Select All
- The Gender filter might not show on the Worksheet: In Gender drop down menu, select Show Filter > a box appears with gender choices for the viewer (Show Me might be blocking).
- We also want to filter by year; drag year to Filter: Again, the Year filter might not show on the Worksheet: In Year drop down menu, click, Show Filter, Dimension and Continuous: Tableau sees the range of values from 1910 to 2012 > click OK
- - In top tool bar (put your cursor on the white canvas) go to the bottom square and find the icon with the square and magnifying glass. It is a zoom tool. Use the very bottom square on the worksheet menu to open up a horizontal tool bar; use zoom control (with the square and magnifying glass) to make the 48 states larger
- We now have a good Sheet 1. But Alaska and Hawaii are scattered making the map small.
 
**Create New Sheets to Make Separate Maps for Alaska and Hawaii**
- In order to make the dashboard more space efficient, we are going to create Hawaii and Alaska as separate maps.
- In bottom or top tool bar, hover over the icons until you find Duplicate Sheet. Sheet 2 will be created.
- As above, in top tool bar (put your cursor on the white canvas) go to the bottom square and find the icon with the square and magnifying glass. It is a zoom tool. Use it to focus just on Hawaii.
- Right click on bottom tab for Sheet 2 and rename -- Hawaii
- Repeat steps and create Sheet 3 named -- Alaska.
- On the main map, zoom into the continental US. Rename Sheet 1 -- 48 states.

**Create the Dashboard**
- Click on top or bottom toolbar for Create New Dashboard
- In left grey sidebar, change size to Automatic. This will affect how your viz is seen on different devices.
- At the bottom of the sidebar, under Objects, change Tiled to Floating. This allows you to move elements around on the Dashboard.
- Drag 48 States to Dashboard. It comes with the year slider, gender filter -- and the entire list of names, which is not necessary. Drag and separate the slider and gender filter from the list of top names. Click on drop down menu for Top Names and select Remove from Dashboard.
- Reposition and make larger the year slider and the gender filter
- Drag Alaska and Hawaii to Dashboard. Remove top names but keep the slider and gender filter 
- If time, eventually we need to have just one year slider and one gender filter for the entire dashboard. 
- - Select the filters of the 48 State Sheet, right click on Filter, select apply to worksheet, select all using related data sources
- Drag and resize until the maps seem right to you

**Adding a title**
- From the left pane, where the sheets are listed, click on text.
- Drag text out into the dashboard. Place it at the very top.
- In the text editor box, write “Baby Name Trends in the US, 1910‐2012”
- Make the text 18pt, bold, and centered.
- Create another text box for your name in smaller type.
- Hit OK.

**Saving the Dashboard and Publishing to the Web**
- Under Server > Tableau Public > Save to Tableau Public As > Choose a descriptive name for your viz page. 
- A pop-up window may appear, saying "Data Extract Required." Click "Create Data Extract" > Extract > Save, and then retry save to Tableau Public.
- There may be a checkbox that says “Show Sheets as Tabs”. But you want people just to see your Dashboard, not the sheets that went into it. Make sure it is unchecked.
- Once your dashboard is saved to the web you will get a preview screen. You’ll see a URL and embed. Copy the embed code, and use it for your GitHub.io page.
