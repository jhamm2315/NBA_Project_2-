# NBAstatsVIS
2016 Utah Visualization Course Final Project

>Project Page URL: https://wilsoncernwq.github.io/NBAstatsVIS/

>Process Book Page URL: https://wilsoncernwq.github.io/NBAstatsVIS/infoPage.html

>Demo Video URL: https://youtu.be/J9vgSrZXdQU

### Motivation
> Visualizing basketball player abilities properly based on statistics is always a hot for sport analysts and basketball fans. There are various basketball data analyzing tools on the internet nowadays, but not many of them can provide user-friendly up-to-date visualizations for general purposes. As basketball enthusiasts, we want to provide such an easy-to-use player profiler for non-experts to explore data and create visualizations based on their own demands.

### Project Structure

We stored files based on file functions:

* [data] - All data files including JSON, CSV, TXT, etc
* [documents] - All documentations of this project, excluding the README.md. The process book is stored inside this folder also
* [external] - All external libraries that we used inside the project. They are *d3*, *d3-hexbin*, *d3-legend*, *d3-queue* and *d3-tip*
* [python] - Python scripts we used for gathering and preprocessing data
* [script] - All JavaScript files wrotten by our group
* [stylesheets] - stylesheets used in this project. The *cssmain.css* is the one wrotten by our group, the rests are generated by the github page.
* [index.html] - The main page of our project
* [infoPage.html] - The information page, where you can find documents including the process book.
* [params.json] - data file generated by the github page.

### Project Features
- You can go to documentation page by clicking "About the Project" link
- Switch player
    - You can switch current player by clicking "Change Player" button
    - You can change filter on the top of the drop-down area
    - You can search the player name by typing key-words in the editable bar
    - You can select player by clicking on its name and the selected player will be displayed
    - You can close the selection menu by clicking "Close Selection"
    - If you have already opened the "Change Player' Menu, the "Compare" button next to it will be disabled automatically until you close the menu 
- Bio-Panel [script/InfoView.js]
    - By default, all the years the player played will be dislayed. You can select a range of years you interested in by brushing on the timeline
    - On the right of the panel, an overall measurement of the player's performance is displayed. The methods of calculating the indices can be found by hover on the tags. The actual career average data can be viewed by hover on the index numbers. The formula for calculating player impact estimation (PIE) can be dound by hover on the PIE tag
    - You can select a attribute name by clicking on corresponding tags. Then views below will be updated based on your selection
- Rank Panel [script/RankView.js]
    - You can hover on the bars to see the focusing view of the data. It shows the actual player ranking of rhe reason your mouse hover on. It shows the ranking number (number after '#'), the player average attribute value of this season (number inside the parentheses) and the player name. There is a star sign in front of the current layer.
- Game Panel [script/GameView.js]
    - This panel shows the player data on each game he played. You can hover on the boxes to see the actual game data. The bar chart on the right and the bottom are two 1D histogram and the main plot is actually a 2D histogram. There are interactions between those three charts.
- Shootting Frequency Panel [script/ShotView.js]
    - This panel shows the shooting frequency of a player on different locations of the court. Colors are used for encoding shooting percentage (% of field goals made verses those attempted). The size of a hexgon represents the number of shoots attempted here, within the years selected before.
    - You can hover on hexgons to view the detail shooting information
    - There are three 1D histograms showing the frequency summary. The plot on the left shows the histogram in terms of shooting distance to the basket. When you hover on this chart, a grey circle will be displayed indicating the range you selected. The actual data will also be dislayed by text on the left of the bar you selected.
    - The plot on the top shows the histogram along the horizontal axis and the histogram on the right shows the vertical axis. You can see the actual data next to the bar you selected.
- Compare Player [script/CompareView.js]
    - You can compare two players in this project
    - By clicking on "Compare" button, you will enter the compare view. You can do query as you did with the "Change Player" mode. By selecting one player, the comparison will be shown below.
    - In this mode, you can not use the "Change Player" button, unless you exit this mode by clicking "Single Player" button
    - You can not brush year in this mode, which was disabled in this mode
    - The bars below shows the comparisons between many attributes of the two players. You can hover on the bars to view their actual data.
    - You can hover on the tag names to see the actual meaning of those attributes

[data]: <https://github.com/wilsonCernWq/NBAstatsVIS/tree/master/data>
[documents]: <https://github.com/wilsonCernWq/NBAstatsVIS/tree/master/documents>
[external]: <https://github.com/wilsonCernWq/NBAstatsVIS/tree/master/external>
[python]: <https://github.com/wilsonCernWq/NBAstatsVIS/tree/master/python>
[script]: <https://github.com/wilsonCernWq/NBAstatsVIS/tree/master/script>
[stylesheets]: <https://github.com/wilsonCernWq/NBAstatsVIS/tree/master/stylesheets>
[index.html]: <https://github.com/wilsonCernWq/NBAstatsVIS/tree/master/index.html>
[infoPage.html]: <https://github.com/wilsonCernWq/NBAstatsVIS/tree/master/infoPage.html>
[params.json]: <https://github.com/wilsonCernWq/NBAstatsVIS/tree/master/params.json>
[script/InfoView.js]: <https://github.com/wilsonCernWq/NBAstatsVIS/tree/master/script/InfoView.js>
[script/RankView.js]: <https://github.com/wilsonCernWq/NBAstatsVIS/tree/master/script/RankView.js>
[script/GameView.js]: <https://github.com/wilsonCernWq/NBAstatsVIS/tree/master/script/GameView.js>
[script/ShotView.js]: <https://github.com/wilsonCernWq/NBAstatsVIS/tree/master/script/ShotView.js>
[script/CompareView.js]: <https://github.com/wilsonCernWq/NBAstatsVIS/tree/master/script/CompareView.js>