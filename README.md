# Excel-Warehouse-Picking-Productivity-Tracker

Interactive Excel workbook to track order picking productivity in a warehouse. Includes password protection and built in reporting and analytics.

# Set Up

Before most of the features of this tracker can be used, information specific to your warehouse need to be saved to the file.
1. Open file and navigate to the Setup sheet. Password protection of this sheet will be enabled by default. Enable editing with the password '6sigma'. 
2. Fill in each picker's name in the Associate column and the corresponding shift each associate works in the shift column. The tables on this worksheet will automatically expand and update references if new rows are added directly beneat them. 
3. Add each outbound carrier for your warehouse in the carrier column along with its corresponding order type (truck load, less than truck load ect).
4. Check that the start times for 2nd shift and new day align with the shcedule at your warehouse. Note that these are the times at which the cut-off between days will be made within the built in reporting and analytics. For example, if the new day start time is set for 2am and a 2nd shift picker is picking at 1am on 1/2/2022, the reporting will register this as part of the 1/1/2022 2nd shift.
5. Update the Order Type and Tires/hr columns. These columns give the standard pick rates for given categories of picks. These rates may be historical, estimated or measured with a time study. These rates will be used to provide information on how pick rates are occurring in comparison to the expected standard. Tires/hr is given as a default example for a tire picking warehouse. This column name can be updated to a more appropriate name for your warehouse such as eaches or cases per hour.
6. Do not edit the Dates column. This column will auto-populate when the first pick is entered into the system.
7. Update the customer column. If this field is not reported for your warehouse, clear the table. This column may be hidden and left blank on the input sheet without interfering with the other features.
8. Save a copy of this file as a template after it's been set up. This file is built to be used for one week at a time. Each new weeek, the template can be copied for a new week. Excel is not able to handle the computational demands of this workbook when it is full or more than a week of picks at a large-scale warehouse. If you are in search of a more powerful tool that can handle longer periods of time, I reccomend using dedicated warehouse management system software.

# Using the Tracker

To begin using the tracker after set up is complete, open the Input sheet. Ensure that macros are enabled. Upon the first entry into the sheet, gray columns and all other sheets will be locked. Double clicking on Time-In or Time-Out will auto-populate it with the current timestamp. These timestamps are also locked after being input. Pick rates input in the Set Up sheet are used to populate the expected time it will take to fulfil each pick. Picks will be color coded with green when they are completed at or below the expected length of time and red when they are not. The remaining sheets show analytics on picking with filtering options. Any inputs may be edited by unlocking the sheet witht he password "6sigma".
