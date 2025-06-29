# Sales Leadership Dashboard

This project is a Sales Leadership Dashboard built using Power BI, PowerApps, and Power Automate, integrated with Dataverse to visualize live sales data and enable dynamic form submissions.

##  Overview

The dashboard fetches real-time data from two Dataverse tables — Employees and Sales — via Direct Query in Power BI. A relationship is established between these tables to drive interactive visuals, including a custom PowerApps form embedded within the report.

Key features include:

•	Live Leaderboard: Ranks top 3 employees based on submitted sales amounts using `RANKX()` in DAX.
•	PowerApps Form: Allows logged-in users to submit their sales, which triggers backend workflows.
•	Automation: On form submission, Power Automate sends an email notification to the admin.
•	Dynamic UI: Includes a visual leaderboard with images and user-specific data inputs.

##Tech Stack

•	Data Source: Dataverse (Direct Query)
•	Dashboard: Power BI  
•	Visuals: Table, Card, PowerApps, Text Box, Image  
•	DAX Functions: `CALCULATE()`, `FILTER()`, `RANKX()`, `SUM()`, `MAX()`
•	Form UI: PowerApps  
•	Controls: Image, Label, InputBox, Button  
•	PowerFx Functions: `Patch`, `Notify`, `Refresh`, `EmailSend.Run`
•	Workflow: Power Automate (Instant triggered from PowerApps)

## How It Works

1. User logs in and views their rank and performance.
2. Enters sales amount via PowerApps form.
3. Submission updates Dataverse and triggers Power Automate.
4. Admin receives an email with the submission info.
5. Leaderboard and report refresh with updated rankings.


 
![image](https://github.com/user-attachments/assets/c8ef0245-5c3e-44a1-8106-8d6493e005b0)

