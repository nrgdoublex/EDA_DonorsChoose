# EDA_DonorsChoose
Data Analysis on DonorsChoose.org

## Description
This project is about the data analysis on datum from <a href="https://www.donorschoose.org/">DonorsChoose</a>, using IPython notebook.  

For the exploratory data analysis part, first we do summary statistics to each column of datum and visualize them, except for text columns. In the second part we check the datum consistency then try to find hidden patterns that may help identify potential donors.

For the time series analysis part, we visualize the time series, then apply ARIMA and LSTM models on these series, trying to explain the patterns.

## Data Descriptions
* `Donations.csv`: 
  + **Project ID**: Unique identifier of a donor.
  + **Donation ID**: Unique ID of a donation.
  + **Donor ID**: The donor’s state.
  + **Donation Included Optional Donation**: Yes/No to give 15% of donation amount to Donoschoose.org.
  + **Donation Amount**: Total amount donated for a project.
  + **Donor Cart Sequence**: Project position on list of desired donations within Cart list.
  + **Donation Received Date**: Date and time on which the donation was received.
* `Donors.csv`:
  + **Donor ID**: Unique identifier of a donor.
  + **Donor City**: The donor’s city.
  + **Donor State**: The donor’s state.
  + **Donor Is Teacher**: Whether or not the donor is also a teacher with a DonorsChoose.org teacher account.
  + **Donor Zip**: The donor’s zip code (only first 3 digits).
* `Projects.csv`:
  + **Project ID**: Unique identifier of a project.
  + **School ID**: Unique identifier of a school where the project is proposed from.
  + **Teacher ID**: Unique identifier of a teacher who proposed the project.
  + **Teacher Project Posted Sequence**: Represents the order as a project issued by the teacher.
  + **Project Type**: Type of the project.
  + **Project Title**: Title of the project.
  + **Project Essay**: Essay of the project.
  + **Project Short Description**: Description of the project.
  + **Project Need Statement**: Statement for the resources that the project needs.
  + **Project Subject Category Tree**: Category of the project.
  + **Project Subject Subcategory Tree**: Subcategory of the project.
  + **Project Grade Level Category**: Grade level that the project aims.
  + **Project Resource Category**: Category of resources that the project needs.
  + **Project Cost**: Costs of the project.
  + **Project Posted Date**: Date when the project is posted.
  + **Project Expiration Date**: Date when the project is expired.
  + **Project Current Status**: Current status of the project.
  + **Project Fully Funded Date**: Date when the project gets fullt funded.
* `Resources.csv`:
  + **Project ID**: Unique identifier of a project.
  + **Resource Item Name**: The name of the requested item, as it appears on the vendor’s website.
  + **Resource Quantity**: The quantity of the requested item.
  + **Resource Unit Price**: The price per unit of the requested item.
  + **Resource Vendor Name**:  Name of the vendor.
* `Schools.csv`:
  + **School ID**: Unique identifier of a school.
  + **School Name**: Name of the school.
  + **School Metro Type**: One of four categories describing metro type, or urbanicity, of school area.
  + **School Percentage Free Lunch**: Integer describing percentage of students qualifying for free or reduced lunch, obtained from NCES data. For schools without NCES data, a district average is used.
  + **School State**: The state of the school that the teacher was teaching at at the time the project was posted.
  + **School Zip**: The zip code of the school that the teacher was teaching at at the time the project was posted.
  + **School City**: The city of the school that the teacher was teaching at at the time the project was posted.
  + **School County**: The county of the school that the teacher was teaching at at the time the project was posted.
  + **School District**: The district of the school that the teacher was teaching at at the time the project was posted.
* `Teachers.csv`:
  + **Teacher ID**: Unique identifier of a teacher.
  + **Teacher Prefix**: “Mrs.”, “Ms.”, “Mr.”, “Teacher” (gender neutral option) chosen by teacher during account creation.
  + **Teacher First Project Posted Date**: Date on which the teacher’s first project was posted.

## File Layouts
* `EDA.ipynb`: Exploratory data analysis part  
* `Time_Series_Analysis.ipynb`: Time series analysis part

## Future
Text analytics section will be added in the future.
