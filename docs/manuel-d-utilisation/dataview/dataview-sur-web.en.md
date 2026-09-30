# Dataview on Web

SC-Dataview on Web lets you view your data and get the full value from it:

- Lets you view up to 8 Tags on the same chart
- Access to real-time data coming from a module
- Saves the parameters of a display and lets you access it in a later session
- Export of data to an Excel spreadsheet for more detailed analysis and to produce your reports

Each combination of tags (maximum 8) can be saved as a "display", which is kept in the SimpliCollect database and can be recalled to show the tags it contains.

Tags are searched in the SimpliCollect database through "tag groups", which simplify the search.  These groups are configured using the SC-Config application (see the Tag Groups topic).

## Step-by-step guide

The functions of the application are as follows:

## Navigation

1.  Once connected to SimpliCollect Web, click the **Dataview** icon to start the application, which appears empty;<br>![Screenshot](../../assets-en/dataview-sur-web/image2020-2-4-10-22-55.png){ width=410 }

2.  Choose one of the displays (1) to access the data of the tags that are part of that display;<br>![Screenshot](../../assets-en/dataview-sur-web/image2020-2-3-20-35-38.png){ width=1024 }

    !!! info

        By default, the time range is 1 hour

3.  For a given display (1), you can change the time span (2) of the data presented on the chart; the different tags that are in the chart are shown at the top of the screen (3), and the data of these tags is shown in the chart (4);

4.  You can change the time range by selecting one of the buttons:  **1h** for 1 hour, **8h** for 8 hours, **1d** for 1 day (24 hours), **1w** for 1 week (7 days) and **1m** for 1 month;<br>![](../../assets-en/dataview-sur-web/dataview-timespan.png)

    !!! info

        When you choose longer time periods, such as a week or a month, the data search takes longer.

5.  The **Refresh ![](../../assets-en/dataview-sur-web/image2020-2-3-20-43-7.png)** button refreshes the content of the chart for the selected time period without changing the selected time range;

6.  The **now ![](../../assets-en/dataview-sur-web/image2020-2-3-20-43-43.png)** button updates the content of the chart starting from now, keeping the selected time span;

7.  You can choose an "ad hoc" time span using the search start and end fields located at the bottom center of the screen:<br>![](../../assets-en/dataview-sur-web/dataview-dates.png)

8.  Choose the start date/time combination and the end date/time combination of the search and click the Refresh button to get the data for that range;

    !!! info

        The maximum time range is limited to 1 month, and the larger the time range, the longer the search will take.

9.  You can also move through time with the forward and backward buttons of the display.  Click the back arrow to go back in time and the forward arrow to go forward in time.<br>![Screenshot](../../assets-en/dataview-sur-web/image2020-2-3-20-52-47.png){ width=704 }

### Tag display

1.  Each tag that is part of the display is shown at the top of the screen and gives the "immediate" data related to the tag:<br>![Screenshot](../../assets-en/dataview-sur-web/dataview-tag-data.png){ width=400 }

### Adding and removing a tag from the display

1.  To add a tag, go to the tag groups section and choose from the various branches of the tree that show the tags:<br>![Screenshot](../../assets-en/dataview-sur-web/dataview-add-tag.png){ width=1024 }
2.  After selecting the tag in the group, it appears at the top of the chart (2) with its current value;<br>![Screenshot](../../assets-en/dataview-sur-web/dataview-add-tag-2.png){ width=1024 }
3.  Click the **Save** button ![](../../assets-en/dataview-sur-web/image2020-2-3-21-19-26.png) to save the added tag in the Display;
4.  To remove a tag from the display, find the tag in the **All Tags** group and uncheck the tag in question (1) to make it disappear from the display (2):<br>![Screenshot](../../assets-en/dataview-sur-web/image2020-2-3-21-22-54.png){ width=1024 }
5.  Click the **Save** button to update the Display.

## Adding a display

1.  Click the **Add ![](../../assets-en/dataview-sur-web/image2020-2-4-9-48-46.png)** button at the bottom of the list of displays and the application responds with a new display ready for configuration:<br>![](../../assets-en/dataview-sur-web/dataview-add-display.png)
2.  Type the name of the display in the field at the top left of the screen, choose whether this display can be shared with other users, and choose whether the items are read-only (i.e. whether another user can change the content of the display):<br>![Screenshot](../../assets-en/dataview-sur-web/dataview-modes.png){ width=500 }
3.  Open a tag group and choose the tags you want to show in the chart:<br>![Screenshot](../../assets-en/dataview-sur-web/image2020-2-4-9-58-33.png){ width=800 }
4.  Click the **Save** button ![](../../assets-en/dataview-sur-web/image2020-2-3-21-19-26.png) to finish creating the new Display:

## Removing a display

1.  In the list of displays, choose the display to remove and click the **Delete ![](../../assets-en/dataview-sur-web/image2020-2-4-10-10-11.png)** button:<br>![Screenshot](../../assets-en/dataview-sur-web/dataview-delete.png){ width=800 }
2.  The application asks you to confirm the removal of the display.  Click **Confirm** to delete the display or **Close** to cancel the deletion;
3.  The display is removed from the SimpliCollect database.

## Export to Excel

Dataview lets you export the data to an Excel file for analysis.

1.  After selecting a display and a time range, with the charts displayed;

2.  Click the **Download CSV** button;<br>![Screenshot](../../assets-en/dataview-sur-web/dataview-csv.png){ width=400 }

3.  The application confirms the creation of the file and starts downloading the CSV file;<br>![Screenshot](../../assets-en/dataview-sur-web/image2020-2-4-10-45-5.png){ width=1024 }

    !!! info

        The file is created in CSV format by the application and will be available in Excel. You can save the file in XLSX format to keep it as an Excel file.<br>The more data points there are in the charts, the longer the download will take, because the file will be large (several megabytes).

4.  Once the download is finished, the file **simplicollect.csv** appears at the bottom of the Chrome web browser and is created in the Downloads folder of your computer;<br>![Screenshot](../../assets-en/dataview-sur-web/image2020-2-4-10-50-37.png){ width=1024 }

5.  The CSV file is in Text format. It is available for analyzing its content with the Excel application, but it can also be opened by any other application that opens Text files.

6.  If a file simplicollect.csv already exists in the Downloads folder, the new file will be named **simplicollect(1).csv**
