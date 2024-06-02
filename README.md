<p align="center">
  <h1 align="center">Getting To Know Microsoft Azure</h1>
</p>

<h2>Links:</h2>

- [Google Doc](https://docs.google.com/document/d/1mN2FS4Fb8lRj2dibaG4J8qsLY0XLnf_WxuumYpzgJr8/edit?usp=sharing)
- [Github Repo](https://github.com/ImranHuhn/AzureBillAlarm)
- [Blog](http://www.techdeficient.com/2024/06/setting-up-billing-alarm.html)

<h2>TLDR: Azure Cost Management</h2>

- <b>Introduction: </b>
  - Azure Cost Management tracks cloud service spending.
  - Budget alerts warn when spending approaches or exceeds limits.
  - Cost alerts notify after exceeding the budget.
  - We will use budget alerts to keep things simple.

- <b>Adding a Budget: </b>
  - Navigate to "Budget" in Cost Management from the Azure portal.
  - Click "Add" to create a new budget.

- <b>Budget Details and Amount: </b>
  - Enter budget details: name, time period (monthly, quarterly, annually), end date, and maximum amount ($200).
- <b>Budget Conditions and Recipients: </b>
  - Set alerts for forecasted and actual spending.
  - Enter email addresses to receive alerts.
  - Click "Create" to finalize settings.

- <b>Budget Completed: </b>
  - Monitor the budget setup progress.
  - Verify the budget appears in Cost Management.
  - Click "Refresh" if it doesn’t appear immediately.

- <b>Conclusion: </b>
  - Setting up budget alerts in Azure helps track and control spending.
  - Follow steps to create and configure budget alerts.
  - Ensure everything is correctly set up to stay informed about spending.


<h2>How to read each section (in this order)</h2>

<b>Section-Intro</b> 
- <b>Title: </b>Name of the section.
- <b>Description: </b>Describe what the section entails. Some sections won’t have descriptions. 

<b>Image</b> 
- <b>Numbering: </b>Within the images are sequential numbers, with corresponding text explanations directly below each image.
- <b>Yellow highlights: </b>Yellow highlights are navigation aids to help identify your current section in the Azure portal.

<b>Text numbers</b> 
- <b>Numbers: </b>Each number provides a brief explanation of the image directly above it.

<b>Side notes</b> 
- <b>Notes: </b>Any extra details you should be aware of.

<h2>Introduction</h2>

&nbsp;&nbsp;&nbsp;&nbsp;Azure Cost Management helps you keep track of how much money you spend on cloud services. There are two types of alerts to help manage your spending: budget alerts and cost alerts. Budget alerts let you know when you're getting close to or have passed your spending limit and can only be set up with billing accounts or billing profiles. Cost alerts tell you after you've gone over your budget. Some cost alerts, like "Reservation Utilization," are only for billing profiles, while others, like "Anomaly" alerts, are only for subscriptions. For our needs, we will only set up budget alerts to keep things simple and stay within our spending limits.


<h2>Adding a budget</h2>

<b>Description: </b>We will start by navigating to the "Budget" section within Cost Management from the Azure portal. Once there, we will initiate the process by adding a new budget. We are now ready to lay the foundation for effective cost management. 

![01Capture](https://github.com/ImranHuhn/AzureBillAlarm/assets/52342912/6700baea-d771-4628-858a-2aa551e66350)

0.  Navigate to the Cost Management section.
1.  Select "Budget" from the left-hand panel.
2.  Click the "Add" button located at the top center of the page.

<h2>Budget details and amount</h2>

<b>Description: </b>In this section, we will enter the budget details, including assigning a label and setting the alert time frame. We will also specify the maximum budget amount, ensuring it aligns with an individual's spending comfort level. By setting these parameters, we create clear guidelines for monitoring and controlling expenses. This approach helps prevent overspending and ensures financial goals are met. Ultimately, these steps enable effective and responsible budget management within Azure Cost Management.

![02Capture](https://github.com/ImranHuhn/AzureBillAlarm/assets/52342912/f318655f-540e-488e-ae4d-e7eb76accd9d)

1.  Enter a name for the budget you are setting up. I named it “two__hunnid”.
2.  Select a time period: monthly, quarterly (every three months), or annually. I chose “Monthly”.
3.  Set an end date for the budget to automatically expire. I picked the farthest year for this example.
4.  Specify the maximum amount you do not want to exceed. I put $200.
5.  Click "Next" once you are satisfied with your entries.

<h2>Budget conditions and recipients</h2>

<b>Description: </b>In this section, we will configure alert conditions to notify you either when it's predicted that you will exceed your budget within the selected timeframe or when you have actually surpassed the budget in real time. This proactive approach ensures you are always aware of your spending status. Next, you'll add at least one email address to receive these alerts, keeping you informed and enabling prompt action. This setup helps you manage your finances effectively and avoid unexpected costs. By staying informed, you can make timely adjustments and maintain control over your budget.

![03Capture](https://github.com/ImranHuhn/AzureBillAlarm/assets/52342912/d57dd8a8-56a4-498f-b8ab-376808b74f57)

1.  Select "Forecast" to receive an alert if your spending is predicted to exceed your chosen amount by the end of the month, quarter, or year. In this case, the budget manager will analyze my resource usage statistics and calculate my probable spending for the rest of the month–since I selected “Month” in the previous section. If this projected amount exceeds your budget, I will be alerted.
2.  Choose the percentage of the budget at which you want to receive a forecast alert. For this example, set it to 100% of $200.
3.  The system will automatically calculate the alert threshold, which in this case is $200.
4.  Additionally, set an actual amount alert to notify you in real-time when the budget is met. In other words, you will only be alerted once the budget has been exceeded.
5.  Like in step 2, choose the percentage of the budget for the actual alert. In this example, set it to 90% of $200.
6.  This will automatically calculate the alert amount based on the percentage from the previous step, which is $180.
7.  Enter at least one email address to receive the alerts.
8.  For this guide I added a second email address for receiving alerts.
9.  Once you are satisfied with the settings, click "Create".

Note: If you see red outlines in the action group section where the “None” dropdown is located, don't worry. This indicates that you need to enter an email address in the alert recipient section below.

<h2>Budget completed</h2>

<b>Description: </b>We will monitor the progress of the budget setup until it is fully completed. Once the budget is established, we will verify its presence in the Azure Cost Management service. This step ensures that the budget is correctly integrated and ready to function as intended. By confirming its setup, we will know that all alerts and notifications are operational. 

![04Capture](https://github.com/ImranHuhn/AzureBillAlarm/assets/52342912/94232881-13d6-4cf0-97c5-d99e81b3b242)

0.  If you're not already in the Budget section within Cost Management, navigate there now.
1.  Click on the bell notification icon to open the right panel.
2.  The right panel will display the status of the budget creation process. Wait until it says "Budget was created".
3.  The new budget should appear in the list. If it doesn't, click the "Refresh" button located next to the "Add" button above.

<h2>Conclusion</h2>

&nbsp;&nbsp;&nbsp;&nbsp;Setting up budget alerts in Azure helps you keep track of your spending on cloud services. We started by navigating to the Budget section and adding a new budget. Then, we named our budget, chose a time period, and set a maximum spending limit. We also set up alerts to notify us if we are predicted to exceed or actually exceed our budget, and added email addresses to receive these alerts. Finally, we ensured everything was set up correctly so we can stay informed and keep our spending under control.
