# Module 8 - Lab 8 - Exercise 1 - Implement a Data Subject Request 

Data subject requests (DSRs) are used to search for and extract all known information on a person of interest. A DSR can come from the person in question or from an authorized source. In this exercise you will configure and export a DSR from the Microsoft 365 Security and Compliance center.

**NOTE:** You should only run a DSR if the request is made by a Data Privacy officer or a Human Resources manager. Due to data privacy legal concerns, you should NEVER run a DSR unless instructed to do so.

### Task 1 – Create a GDPR Data Subject Request

Holly Dickson is Adatum’s Enterprise Administrator. In her role as the company’s Microsoft 365 Global Administrator, she is responsible for implementing Adatum’s Microsoft 365 pilot project. Since Adatum has several European subsidiaries, properly managing GDPR data subject requests is a key task that must be tested so the company can successfully implement this feature in accordance with EU law. In this task, Holly will create a DSR for herself on behalf of a request made by the Human Resource department.

**Note:** To perform this task, Holly must be assigned to the eDiscovery Manager role group so that she has the necessary permissions. You added Holly to this role group in Lab 1 at the same time that you added Joni Sherman to the role group. The reason why you were instructed to add Holly to the eDiscovery Manager role group in Lab 1 rather than at the start of this lab is that it takes several minutes for permissions to successfully propagate. If you had assigned Holly to this role group just prior to this query, you would have received error messages involving parameter fields because her permissions would not have completed propagating. By adding Holly to this role group at the start of this course, enough time will have elapsed between then and now for the propagation to complete. 

1. Switch to LON-CL1, where you should still be logged in as the **Admin** account, and you should be logged into Microsoft 365 as **Holly Dickson** (**holly@M365xZZZZZZ.onmicrosoft.com)** with a password of **Pa55w.rd**. 

2. In your **Microsoft Edge** browser, if you have the **Security and Compliance Center** open in a tab, then select it; otherwise, open a new tab and enter the following URL in the address bar: **https://protection.office.com**.

3. In the **Security and Compliance center**, in the left-hand navigation pane select **Data privacy**, and then under it select **Data subject requests**.  

4. In the **Data subject requests** window, select **+New DSR case**. This initiates the **New DSR case** wizard.

5. In the **Name your case** page, enter the following information and then select **Next**:

	- Name: **Holly Dickson Subject Request**

	- Description: **This is a test of the DSR resource to pull info on Holly Dickson.**

6. In the **Request details** page, select the **Data subject (the person who filed this request)** field, which displays a list of users. Select **Holly Dickson** and then select **Next**.

7. In the **Confirm your case settings** page, review your settings. If necessary, select **Edit** next to either setting to change it. If everything looks correct, select **Save**.

8. In the **Successfully created new DSR case** window, select **Show me search results**.

9. A new **Search query** window will appear and begin the query. In the detail pane on the left, scroll to the bottom, where the **Status** of the query is displayed. Wait for the status to show **Completed**.  <br/>

	‎**Note:** Depending on how much data is accrued, a query can take some time to complete. For Adatum’s pilot project, they have not accrued much in the way of data, so Holly Dickson’s query should only take a minute or so to complete.

10. At any point, scroll down under **Search query** in the left-hand pane to review the default query parameters. You can modify any of the parameters and save the query for future use. If you modify any of the parameters, select **Save**.

11. Select the **Home** tab. For Holly Dickson’s case, select **Close case** to the right of the **Active** status, and then select **Yes** on the **Warning** message. 

12. In the **Searches** tab, open the saved search selecting the check box next to **Holly Dickson Subject Request**. 

13. In the **Holly Dickson Subject Request** window, scroll to the bottom of the window to view search statistics of the results as well as the search query syntax. 

14. Leave this **Holly Dickson Subject Request** window open as you will resume testing in the next task from this point.

You have created a data subject request and you have searched for the personal information of Holly. At the end of your test, you have closed the DSR case again. 


### Task 2 – Export the DSR Search Query Results

When someone files a DSR, you typically need to export the results. In this task, Holly will export the DSR report for the previous case for further processing.

1. The **Holly Dickson Subject Request** window should still be open after having finished the previous task. At the top of the pane, select the **Export report** button.

3. In the **Export report** window, select the option that states: **All items, including ones that have unrecognized format, are encrypted, or weren’t indexed for other reasons**.  <br/>

	**Note:** Be careful - The first two options appear at first glance to be similar; however, the first one **excludes** items while the second one **includes** those same items. Select the second option.

4. Scroll down through the **Export report** window to see the estimated items that will be exported. 

5. Select **Generate report**.

6. If a **Client Error** dialog box appears, select **OK**. 

7. When the report finishes, select **Close**. 

8. Select the **Exports** tab from the top menu and select the **Holly Dickson Subject Request_ReportsOnly** export request to open it.

9. In the right-hand pane select the **Download report** button. In the notification bar that appears at the bottom of the page, select **Open**.

10. An **Application Install – Security Warning** window will appear that wants to install the **Microsoft 365 Office 365 eDiscovery Export Tool**. Select the **Install** button.

11. When the **eDiscovery Export Tool** is installed, you need to copy the unique export key to the first text field. Go back to the **Holly Dickson Subject Request_ReportsOnly** export request window in your browser and below **Export key**, select **Copy to clipboard**.

12. Switch back to the **eDiscovery Export Tool** (select the corresponding icon on your taskbar) and paste the export key (press **Ctrl+V**) into the first text field.

13. Select the **Browse** button next to the **Select the location that will be used to store downloaded files** field, and in the **Browse For Folder** window, navigate to **Documents**. Select **OK**.

14. Select **Start** to begin the export process.

15. As soon as the **eDiscovery Export Tool** shows three green checkmarks with a **The export completed successfully** message below them, the export is done. Select the link that appears next to **Export Location**.

16. This opens a **File Explorer** window. Double-click the **results.csv** file to open Excel and view the report data for all DSR case items found. When you're done, close the Excel spreadsheet and then close the **File Explorer** window.

17. Close the **eDiscovery Export Tool** by selecting the **Close** button, and then close the **Holly Dickson Subject Request_ReportsOnly** window.

18. In your browser, close the **eDiscovery** tab and the **Data subject requests - Security and Compliance** tab.

18. Leave **Holly** signed in at the **Security &amp; Compliance Center**.

You have successfully exported a DSR case report to your local computer. Note: Because the report contains only a report and not the message or document content, you could not process this report to fulfill the DSR's legal requirements.


# Proceed to Lab 8 - Exercise 2
