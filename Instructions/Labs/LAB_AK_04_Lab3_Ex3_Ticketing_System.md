<h1>Module 4 - Lab 3 - Exercise 3 - Create a Ticketing System in SharePoint </h1>
<p>As Adatum begins its transition to Microsoft 365 as their hosted cloud solution, they want to use this opportunity to reduce the amount of third-party software products they currently use. This will help them achieve their goal of reducing their overall IT expenses. The CTO has asked Holly Dickson, Adatum&rsquo;s Enterprise Administrator, to design a solution that uses Microsoft 365 services to replace the third-party IT service request system that Adatum currently uses.</p>
<p>Because Holly is busy with running the Microsoft 365 pilot project along with her other admin responsibilities, the CTO has authorized her to hire an IT consultant to design the new service request ticketing system. However, he doesn&rsquo;t want the consultant to have access to their entire Adatum system, so he wants Holly to implement &ldquo;good security practices&rdquo; by only providing the consultant with access to Adatum&rsquo;s IT pilot project environment.</p>
<h2>Important: Collaboration with an External User</h2>
<p>In Lab 1, your instructor assigned you the tenant suffix ID of a fellow student in your class. Your fellow student's tenant ID will represent the IT Consultant who will partner with Holly Dickson in building Adatum's new service request ticketing system. In this lab, you will provide your fellow student's tenant ID with access to the new ticketing system. In a lab 1 exercise, you authorized external access to your tenant from this student&rsquo;s tenant ID. By providing external access to this tenant suffix ID, you and your fellow student will be able to collaborate through Microsoft Teams as you set up this new service request ticketing system (you will do this in the next lab that deals with Teams).</p>
<p>In the previous lab exercise, you created a SharePoint team site called IT Services. As you develop this site, you will employ good security practices by limiting site access to Holly and your fellow student's tenant ID (this tenant ID represents the IT consultant). As you set up the new service request ticketing system, you will access the site using your fellow student's tenant ID to prove that the IT consultant can access the system. In the next lab involving Microsoft Teams, you will actually chat with your fellow student concerning the new ticketing system. Keep in mind that the student who was assigned as your IT consultant will also be taking on the role of Holly Dickson in his or her own lab, and you will be taking on the IT consultant role with another student. Therefore, each student in the class will take on dual roles &ndash; that of Holly Dickson in the student&rsquo;s own lab, and that of the IT consultant for a fellow student&rsquo;s lab.</p>
<h3>Task 1 - Assign site permissions to your IT consultant</h3>
<p>As Holly Dickson, you earlier provided your fellow student's tenant ID with External Access back in Lab 1. You now must assign the consultant with permission to access the new IT Services team site that you created in the prior lab. If you will recall, in the prior lab you created a new Information Technology group that was assigned to the IT Services site. This group included Isaiah Langer and Joni Sherman, and you assigned the group Full Control permissions. Since you do not want the IT consultant to have Full Control permissions, you do not want to assign the consultant to the Information Technology group.</p>
<p>Instead, in your role as Holly Dickson, you will perform the following steps in this task to assign the IT consultant to the IT Services team site with limited permissions:</p>
<ul>
<li>You will create a new permission level for the IT Services site titled <strong>Restricted Use</strong>. You will then assign to this permission level the limited set of permissions that you want assigned to any external users who will access the site (in this case, the IT Consultant).</li>
<li>For the IT Services site, you will then create a new group of users titled <strong>Consultants</strong>, and you will assign your fellow student&rsquo;s tenant admin account (which represents the IT Consultant) to this group.</li>
<li>You will assign the <strong>Restricted Use </strong>permission level to this <strong>Consultants</strong> group. This will limit the actions the IT Consultant will be able to perform when accessing the IT Services site.</li>
</ul>
<ol>
<li>You should meet with the student who your instructor assigned to your lab to play the role of the IT consultant. During this meeting you should exchange the tenant admin accounts <strong>(admin@xxxxxZZZZZZ.onmicrosoft.com) </strong> from each of your tenants along with the tenant admin's password.</li>
<li>You should still be logged into LON-DC1 as <strong>ADATUM\Administrator</strong> and password <strong>Pa55w.rd</strong>; if not, then do so now.</li>
<li>You should still have your Edge browser and the SharePoint admin center open from the prior lab in which you were logged in as Holly Dickson. If so, proceed to the next step; otherwise, navigate to the SharePoint admin center just as you did in the prior lab exercise.</li>
<li>In the <strong>SharePoint admin center</strong>, you will begin by creating a new permission level for the IT Services site. In the left-hand navigation pane, select <strong>Sites</strong>, and then select <strong>Active sites</strong>.</li>
<li>In the list of <strong>Active sites</strong>, locate the <strong>IT Services </strong>site and then select the<strong> &hellip;/sites/ITServices</strong> value that appears in the URL column for this site.</li>
<li>A new tab will open in your Edge browser that displays the <strong>IT Services</strong> site. In the upper right-hand corner of the <strong>IT Services</strong> site, select the <strong>gear (Settings)</strong> icon.</li>
<li>In the <strong>Settings</strong> pane that appears, select <strong>Site permissions.</strong></li>
<li>At the bottom of the <strong>Site permissions</strong> pane, select <strong>Advanced permissions settings</strong>, which opens a <strong>Permissions: IT Services</strong> page.</li>
<li>In the ribbon that appears at the top of the screen, the <strong>PERMISSIONS</strong> tab is displayed by default. Under the <strong>Manage</strong> section, select <strong>Permission Levels.</strong></li>
<li>In the <strong>Permissions &gt; Permission Levels</strong> page, on the menu bar that appears above the list of permission levels, select <strong>Add a Permission Level</strong>.</li>
<li>In the <strong>Permission Levels</strong> &gt; <strong>Add a Permission Level</strong> page, enter the following information:
<ul>
<li>Name: <strong>Restricted Use</strong></li>
<li>Description: <strong>This level restricts the level of use inside the IT Services site.</strong></li>
<li>When selecting the permissions, do NOT select the <strong>Select All</strong> Instead, select the following limited set of permissions under the <strong>List Permissions</strong> section:
<ul>
<li><strong>Manage lists</strong> (which selects <strong>View Items</strong>)</li>
<li><strong>Add items</strong></li>
<li><strong>Edit items</strong></li>
<li><strong>View versions </strong>(which selects <strong>Open Items</strong>)</li>
<li><strong>View Application Pages</strong></li>
</ul>
</li>
<li>Select the following permissions under the <strong>Site Permissions</strong> section:
<ul>
<li><strong>Add and Customize Pages</strong> (which selects<strong> Browse Directories, View Pages</strong>, and<strong> Open</strong>)</li>
<li><strong>Use Self-Service Site Creation </strong>(which selects <strong>Browse User information</strong>)</li>
<li><strong>Use Remote interfaces</strong></li>
<li><strong>Use Client integration features</strong></li>
</ul>
</li>
</ol>
<ol start="12">  
<li>Scroll to the bottom of the page and select the <strong>Create </strong>button to create the new<strong> Restricted Use </strong>permission level.</li>
<li>Once the permission level is created you will be redirected to the<strong> Permissions</strong> &gt; <strong>Permission Levels</strong> page. Verify the new <strong>Restricted Us</strong>e permission level appears in the list of permission levels for this IT Services site. 
  <br><br>On this <strong>Permissions</strong> &gt; <strong>Permission Levels</strong> heading line, select the <strong>Permissions </strong>link to return to the <strong>Permissions: IT Services</strong> page.</li>
<li>In the ribbon displayed at the top of the screen, the <strong>PERMISSIONS </strong>tab is displayed by default. In this tab, under the <strong>Grant</strong> section, select <strong>Create Group</strong>.</li>
<li>On the <strong>People and Groups &gt; Create Group</strong> page, enter the following information:
<ul>
<li>Name<strong>: Consultants</strong></li>
<li>About Me<strong>: This group is used for allowing consultants to modify work products only</strong>.
<li>Who can view the Membership of the Group<strong>: Everyone</strong></li>
<li>Who can edit the membership of the Group<strong>: Group Owner</strong></li>
<li>Allow requests to Join/leave this group<strong>: No</strong></li>
<li>Auto-accept requests: <strong>No</strong></li>
<li>Choose the permission level group members get on this site:<strong> Restricted use &ndash; This level restricts the level of use inside the IT Services site </strong>
<br><br><strong>Note: </strong>This setting includes the<strong> Designer </strong>permission level that you created in the prior lab and the<strong> Restricted Use </strong>permission level that you just created in this task. You will only assign this group the <strong>Restricted Use </strong>permission level.</li>
</ul>
</li>
<li>Select <strong>Create</strong>. You will be redirected to the <strong>People and Groups</strong> &gt; <strong>Consultants</strong> page for this <strong>Consultants</strong> group.</li>
<li>On the menu bar that appears above the list of consultants, select the drop-down arrow next to <strong>New</strong>. In the menu that appears, select <strong>Add Users.</strong></li>
<li>In the <strong>Share &lsquo;IT Services&rsquo;</strong> window that appears, in the <strong>Enter names or email addresses </strong>field, enter your fellow student&rsquo;s tenant admin account, which will be <strong>admin@xxxxxZZZZZZ</strong><strong>.onmicrosoft.com</strong> (<strong>IMPORTANT:</strong> replace xxxxxZZZZZZ with your fellow student&rsquo;s tenant prefix that was assigned to you by your instructor; do <strong>NOT</strong> use your tenant prefix). 
<br><br>This same address will be displayed below the field in a menu. Select this address.
<br><br><strong>Note: </strong>A message should appear below this field that says: <strong>admin@xxxxxZZZZZZ</strong><strong>.onmicrosoft.com is outside of your organization.</strong></p></li>
<li>Select <strong>SHOW OPTIONS. </strong>Note that the <strong>Send an email invitation</strong> option is selected by default. Leave this option selected.</li>
<li>Select <strong>Share</strong>.</li>
<li>Because you selected the option to <strong>Send an email invitation</strong>, your fellow student will receive an email invitation in his or her MOD Administrator&rsquo;s Inbox. To verify this email was received, you must open an InPrivate browsing session to impersonate your fellow student&rsquo;s tenant. This enables you to access your fellow student&rsquo;s MOD Administrator account within the student&rsquo;s tenant, and therefore access this MOD Administrator&rsquo;s Outlook Inbox.
  <br><br>On your taskbar, right-click on the <strong>Microsoft Edge</strong> icon and select <strong>New InPrivate window</strong> in the menu that appears.</li>
<li>This opens an InPrivate browsing session. Maximize the InPrivate browser window, and then enter the following URL in the address bar: <strong>https://outlook.office365.com/mail/inbox</strong></li>
<li>In the <strong>Sign in</strong> window, enter your fellow student&rsquo;s MOD Administrator email address of <strong>admin@xxxxxZZZZZZ</strong><strong>.onmicrosoft.com</strong> (where xxxxxZZZZZZ is your fellow student&rsquo;s tenant prefix that was assigned to you by your instructor). In the <strong>Enter password</strong> window, enter your fellow student's tenant email password and select <strong>Sign in</strong>.</li>
<li>In the <strong>Stay signed in?</strong> dialog box, select <strong>Yes</strong>.</li>
<li>This will open your fellow student&rsquo;s MOD Administrator&rsquo;s Inbox in Outlook. In the Inbox you should see an email from <strong>no-reply@sharepointonline.com. </strong>Open the email.</li>
<li>In the email, it will display <strong>Go To</strong> <strong>IT Services</strong>. The<strong> IT Services </strong>portion of this message is hyperlinked. Select <strong>IT Services</strong>.</li>
<li>A new tab will open in your InPrivate browsing session that displays <strong>Welcome to SharePoint Online. </strong>On this webpage, select <strong>Organizational account. </strong></li>
<li>This will open the <strong>IT Services</strong> site that you created in your tenant. In other words, by using an InPrivate browsing session, you are impersonating your fellow student by being signed into his or her tenant, and from your fellow student&rsquo;s browser (i.e. in the InPrivate browsing session), you are accessing the <strong>IT Services</strong> site that Holly created in Adatum&rsquo;s Microsoft 365 tenant.</li>
<li>On the <strong>IT Services</strong> site, in the left-hand navigation pane, select <strong>Documents</strong>.</li>
<li>On the <strong>Documents</strong> page, select <strong>+New</strong> on the menu bar. In the drop-down menu that appears, you should see all the objects the IT Consultant can create in this site.</li>
<li>Select the X in the upper right corner of the screen to close the InPrivate Browsing session in Microsoft Edge.</li>
<li>Close the Microsoft Outlook mail message that you opened earlier. </li>
<li>This will return you to the <strong>People and Groups &gt; Consultants</strong> site in your normal Edge browser session. If your fellow student's MOD Administrator account does not appear in the list of consultants, select the <strong>Refresh</strong> icon on the left-side of the address bar at the top of the page to refresh the list. Your fellow student's <strong>MOD Administrator</strong> account should now appear. </li>
<li>Leave the browser open and proceed to the next task.</li>
</ol>
<h3>Task 2 - Upload existing ticket request data (<strong>IT Consultant steps</strong>)</h3>
<p>In this task, <strong>you will take on the persona of the IT consultant</strong> who is helping Holly Dickson implement a new service request ticketing system. In your role as the IT consultant, you are concerned that during this transition from Adatum&rsquo;s old ticketing system to the new one, Adatum may lose critical historical data, such as ticket volume and monthly activity. Therefore, you have recommended to Holly that you should upload the existing data from Adatum&rsquo;s old service request ticketing system to the new ticketing system.</p>
<p>To facilitate this process, the existing ticketing data has been captured in a spreadsheet and a backup spreadsheet, and your lab service provider has stored these two spreadsheets on LON-CL1. </p>
<p>As the IT Consultant in this task, you will perform two primary steps:</p>
<ul>
<li>You will connect to Adatum&rsquo;s IT Services team site to validate that you can access the site and authenticate your credentials.</li>
<li>You will export the existing ticket data from the spreadsheet on LON-CL1 and upload it to a SharePoint list in the IT Services site that Adatum (Holly) created in the prior task. When the data is uploaded to the IT Services site, it will be uploaded as a SharePoint list (titled &ldquo;Service Desk Requests&rdquo;) on the site. 
  <br><br><strong>IMPORTANT: </strong>There are two ways in which you can export the data from the spreadsheet and upload it to the SharePoint list on the IT Services site: through commands in the Excel spreadsheet, or by running a PowerShell script. Both options are presented in this task and you are free to choose whichever method you prefer. Using the Excel spreadsheet commands is probably the more common method, but for those of you who prefer to work in PowerShell, using the PowerShell script provides another experience to add to your personal repository of PowerShell tools.</li>
</ul>
<p><strong>CAUTION:</strong> In this task, whenever you access the URL of the IT Services site, you will use <strong><u>your</u></strong> tenant prefix (xxxxxZZZZZZ) in the URL (<strong>https://xxxxxZZZZZZ.sharepoint.com/sites/ITServices</strong>), since you created the site in your Adatum tenant in the prior task. When you access this site in your role as the IT Consultant, you will sign in using your fellow student's tenant admin username and password (which represents the IT Consultant); the username will be <strong>admin@xxxxxZZZZZZ.onmicrosoft.com</strong>, where the tenant prefix (xxxxxZZZZZZ) will be <strong><u>your fellow student&rsquo;s</u></strong> tenant prefix that was assigned to you by your instructor.</p>
<ol>
<li>Switch to <strong>LON-CL1</strong>.</li>
<li>On <strong>LON-CL1</strong>, you should still be logged in as the <strong>Administrator</strong> (Adatum\Administrator) from the earlier lab in which you installed Microsoft 365 Apps for enterprise. If you did not log out of LON-CL1 as Laura Atkins and log back in as the Administrator at the end of the earlier lab, then do so now.
<li>Select the <strong>File Explorer</strong> icon that is located on the taskbar at the bottom of the screen.</li>
<li>Maximize the <strong>File Explorer</strong> window, and then select the <strong>Documents</strong>.</li>
<li>If you will recall from the task description, you will be presented with two options for completing this task: through commands in the Excel spreadsheet, or by running a PowerShell script. 
  <ul>
    <li>If you prefer to use Excel to accomplish this task, then proceed to <strong>step 6</strong>. </li>
    <li>If you prefer to use PowerShell, then proceed to <strong>step 25</strong>.</li>
  </ul>
  </li>
<br><br>
<li><strong>START HERE TO PERFORM THIS TASK USING EXCEL.</strong> 
  <br><br>Since you are at this step, you have chosen to use Excel to export the table data into a SharePoint list in the IT Services site. 
  <br><br>Confirm that the <strong>Service Request System.xlsx </strong>and <strong>BackupFile.xlsx</strong> files are present in the<strong> Documents</strong> folder. The <strong>Service Request System</strong> spreadsheet contains copies of the service request tickets from Adatum&rsquo;s old ticketing system. The <strong>Backup File</strong> spreadsheet, which is simply a copy of the Service Request System file, was created for precautionary purposes (it will come into play in the next task). Note that there are two files with the name <strong>Service Request System</strong>; one is an Excel spreadsheet file with a .xlsx extension, and the other is a comma separated value file with a .csv extension. The Excel spreadsheet file is used in this section, whereas students that chose to use PowerShell will use the .csv file.
  <br><br>Double-click the <strong>Service Request System.xlsx </strong>file to open it. Make sure you open the .xlsx file and not the .csv file. </li>
<li>If a <strong>Sign in to set up Office</strong> window appears, sign in using the tenant admin account (admin@xxxxxZZZZZZ.onmicrosoft.com, where xxxxxZZZZZZ is the tenant prefix provided by your lab hosting provider) and tenant admin password. </li>
<li>If an <strong>Accept the license agreement</strong> window appears, select the <strong>Accept</strong> button.</li>
<li>If a <strong>Your privacy option</strong> window appears, select the <strong>Close</strong> button at the bottom of the window.</li>
<li>In the next several steps, you will verify that in your role as the IT Consultant, you can connect to the IT Services site and that you can authenticate access to the site using your tenant admin&rsquo;s credentials. Even though you will use the Excel command to <strong>Get Data</strong> from another source and import it into your spreadsheet, you will actually NOT being doing that since you already have the data in the spreadsheet. You will simply use this <strong>Get Data </strong>command to verify that you can successfully access the IT Services site from your PC. 
  <br><br>In <strong>Excel,</strong> in the menu bar at the top of the screen, select <strong>Data</strong>.</li>
<li>In the ribbon, under the <strong>Get and Transform Data</strong> section, select the <strong>Get Data </strong>drop-down arrow. In the menu that appears, select <strong>From Online Services</strong>, and then in its menu, select <strong>From SharePoint Online list</strong>.</li>
<li>A new <strong>SharePoint Online lists</strong> window will open. In the <strong>Site URL</strong> field, enter <strong>https://xxxxxZZZZZZ.sharepoint.com/sites/ITServices</strong> (where xxxxxZZZZZZ is the tenant prefix provided by your lab hosting provider, since the IT Services site is on your tenant). 
  <br><br><strong>Note: </strong>Before you select <strong>OK</strong>, copy the site URL that you just entered as you will need to enter this in future steps. Copying it now will save you from having to manually enter it later. 
  <br><br>Select <strong>OK</strong>.</li>
<li>If a dialog box appears that allows you to select the type of authentication you want to use to access the IT Services site, it will display three options in the left-hand pane: Anonymous, Windows, and Microsoft account. Anonymous is displayed by default. However, in this case, select <strong>Microsoft account</strong>.
<br><br>The dialog box displays a message indicating <strong>You aren&rsquo;t signed in</strong>. Select the <strong>Sign in</strong> button.
<br><br>On the <strong>Pick an account</strong> window, select <strong>Use another account</strong> because you want to sign in as the IT Consultant's tenant admin account (<strong>admin@xxxxxZZZZZZ.onmicrosoft.com</strong> where xxxxxZZZZZZ is <strong>your fellow student&rsquo;s tenant prefix that was assigned to you by your instructor</strong>). In the <strong>Enter password</strong> window, enter your fellow student's tenant password and then select <strong>Sign in</strong>. If your sign in is successful, a message will be displayed in the window indicating you are signed in.
<br><br>Once you are signed in, select <strong>Connect</strong>.</li>
<li>When the <strong>Navigator</strong> window appears, this is your indication that you have established a connection between the IT Consultant&rsquo;s external user account and Adatum&rsquo;s IT Services site that Holly created in the prior task. Even though you used the <strong>Get Data</strong> command in Excel to do this, you will NOT import any data locally to the Excel spreadsheet (the data is already in the spreadsheet).
  <br><br>Select <strong>Cancel</strong> to close the <strong>Navigator</strong> window. </li>
<li>Now that you have verified that the IT Consultant's external user account can access the IT Services site, you will export Adatum&rsquo;s existing ticketing system data from the spreadsheet and upload it as a SharePoint list into the IT Services site. 
  <br><br>If you are already familiar with the use of table objects in Excel, <strong>select a cell in the table and proceed to the next step.</strong> 
  <br><br>However, if you are not that familiar working with tables in Excel, note how the final two menu bar options are <strong>View</strong> and <strong>Help</strong>. You are now going to select the table in the spreadsheet, and after doing so, you will note the changes to the menu bar. 
  <br><br>Before you can export an Excel table into a SharePoint list, the stationary list of data must be inserted into an Excel table object. This has already been done for you as the data in the spreadsheet has already been inserted into an Excel table object. All you must do now is select the table, which can be done by simply selecting any cell of data (for example, select cell <strong>C3</strong>). 
  <br><br>Because you have now selected the Excel table, note how the new menu bar option titled <strong>Table Design</strong> appears after <strong>Help</strong>. 
  <br><br><strong>Note:</strong> If you select a cell outside of the table, note how the <strong>Table Design</strong> menu bar option disappears. If you once again select a cell inside the table, note how it reappears.</li>
<li>On the menu bar, select <strong>Table Design</strong>.</li>
<li>In the ribbon, under the <strong>External Table Data</strong> section, select the <strong>Export </strong>drop-down arrow. In the menu that appears, select <strong>Export Table to SharePoint List</strong>.</li>
<li>An <strong>Export Table to SharePoint List &ndash; Step 1 of 2</strong> window will appear. Enter the following information:
<ul>
<li><strong>Address:</strong> If you copied the IT Services site URL from the earlier step, then paste that in now; otherwise, enter <strong>https://xxxxxZZZZZZ.sharepoint.com/sites/ITservices</strong> (where xxxxxZZZZZZ is <strong>your tenant prefix</strong> provided by your lab hosting provider). 
  <br><br><strong>Important:</strong> By default, the Address field is prefilled with &ldquo;http://&rdquo;. If you manually enter the URL, you must change this to &ldquo;https://&rdquo;; otherwise, your connection to the IT Services site will fail.</li>
<li><strong>Name:</strong> This is the name of the new distribution list that will be created in this site. For Adatum's new ticketing system, enter <strong>Service Desk Requests</strong>.</li>
<li><strong>Description:</strong> (optional) &ndash; leave blank</li>
</ul>
</li>
<li>Select <strong>Next</strong>.</li>
<li>An <strong>Export Table to SharePoint List &ndash; Step 2 of 2</strong> window will appear. Review the information and then select <strong>Finish</strong>.</li>
<li>A <strong>Microsoft SharePoint Foundation</strong> dialog box will appear that indicates the table was successfully published. 
  <br><br><strong>Important:</strong> Do NOT select OK; instead, select the <strong>link</strong> to the site in which the table was published. This will take you to the IT Services site where it will display a list showing the data that was exported from the spreadsheet and uploaded into the site. 
  <br><br><strong>Note:</strong> If a <strong>Sign in</strong> window appears, enter the MOD Administrator&rsquo;s account for the IT Consultant&rsquo;s tenant. In this case, enter <strong>admin@xxxxxZZZZZZ.onmicrosoft.com</strong> (where xxxxxZZZZZZ is your fellow student's tenant prefix that was assigned to you by your instructor). Select <strong>Next</strong>, and then in the <strong>Enter password</strong> window, enter your fellow student's tenant password and then select <strong>Sign in</strong>.</li>
<li>On the taskbar at the bottom of the screen, select the <strong>Excel</strong> icon. In the <strong>Microsoft SharePoint Foundation</strong> dialog box that displayed the link to the published list in the IT Services site, select <strong>OK</strong> to close the window. </li>
<li>Close Excel. </li>
<li>Close your Edge browser. 
  <br><br><strong>Important:</strong> This completes the steps involved in using Excel to export the table data into a SharePoint list (Service Desk Requests) in the IT Services site. <strong>You should SKIP the remaining steps in this task and proceed to the next task.</strong>
<br><br></li>
<li><strong>START HERE TO PERFORM THIS TASK USING POWERSHELL. </strong>
  <br><br>Since you are at this step, you have chosen to use Windows PowerShell to export the table data into a SharePoint list in the IT Services site rather than using Excel to accomplish this task. 
  <br><br>Confirm that the <strong>Service Request System.csv </strong>file is present in the<strong> Documents</strong> folder. This file contains copies of the service request tickets from Adatum&rsquo;s old ticketing system. 
  <br><br>Confirm that the <strong>ImportCsvToSharepointList.ps1</strong> script is present in the <strong>Documents</strong> folder. This script contains the PowerShell commands you will run to export the table data from the <strong>Service Request System.csv </strong>file and import it into a SharePoint list in the IT Services site.</li>
<li>In the <strong>Search</strong> field on the taskbar at the bottom of the desktop, enter <strong>PowerShell</strong>. 
  <br><br><strong>Important: </strong>Because you MUST run several of the commands within this script individually rather than running the entire script at once, you should select <strong>Windows PowerShell ISE </strong>(not Windows PowerShell); therefore, right-click on <strong>Windows PowerShell ISE</strong> and select <strong>Run as administrator</strong>.</li>
<li>If a <strong>User Account Control</strong> dialog box appears, select <strong>Yes </strong>to allow this app to make changes to your device.</li>
<li>In <strong>Windows PowerShell ISE</strong>, in the menu bar, select <strong>File </strong>and then select <strong>Open</strong>. Navigate to <strong>This PC</strong> and then to the <strong>Documents</strong> folder. Select the <strong>ImportCsvFileToSharepointList</strong> script and then select <strong>Open</strong>.</li>
<li>In the script, you will run the commands in lines <strong>11-13</strong> together; therefore, select these three lines in the script and then select the <strong>Run Selection (F8)</strong> icon on the menu bar. These lines will set your execution policy as Remote Signed and install both the SharePoint Online module as well as the SharePoint PNP module. The PNP module enables you to remotely sign into your SharePoint Online environment and manage your SharePoint lists.</li>
<li>If you are prompted to confirm an <strong>Execution Policy Change</strong>, select <strong>Yes to All.</strong></li>
<li>If you are prompted to confirm a <strong>NuGet provider is required to continue</strong>, select <strong>Yes</strong>.</li>
<li>If you are prompted to confirm an <strong>Untrusted repository</strong>, select <strong>Yes to All.</strong></li>
<li>If you are prompted a second time to confirm an <strong>Untrusted repository</strong> dialog box, select <strong>Yes to All.</strong></li>
<li>At the command prompt, you will run the commands in lines <strong>20-21</strong> together; therefore, select these two lines in the script and then select the <strong>Run Selection (F8)</strong> icon on the menu bar.</li>
<li>In the <strong>Windows PowerShell credential request</strong> dialog box that appears, enter <strong>admin@xxxxxZZZZZZ.onmicrosoft.com</strong> in the <strong>User name</strong> field (where xxxxxZZZZZZ is the tenant prefix <u>from your fellow student</u> that was assigned to you by your instructor); this is the IT Consultant&rsquo;s MOD Administrator (tenant admin) account.
  <br><br><strong>Note:</strong> Copy the value (Ctrl+C) that you entered in the <strong>User name</strong> field as you will have to enter it again in a couple of steps. By copying the value here, you can simply paste it in later on rather than re-entering it. 
  <br><br>Enter your fellow student's tenant admin password in the <strong>Password </strong>field, and then select <strong>OK</strong>.</li>
<li>On line <strong>32</strong> in the script, you MUST update the URL before you can run this command. In the URL, you must replace the xxxxxZZZZZZ with <u>your tenant ID</u> provided by your lab hosting provider (this is your Adatum tenant where the IT Services site was created earlier by Holly).</li>
<li>At the command prompt, you will run the command in line <strong>32 </strong>by itself; therefore, select this line in the script and then select the <strong>Run Selection (F8)</strong> icon on the menu bar.</li>
<li>In the <strong>Enter your credentials</strong> dialog box, paste into the <strong>User name</strong> field the value that you copied in the earlier step. If you did not copy the User name value, then enter in the <strong>User name</strong> field <strong>admin@xxxxxZZZZZZ.onmicrosoft.com</strong> (where xxxxxZZZZZZ is the tenant prefix <u>from your fellow student</u> that was assigned to you by your instructor); this is the IT Consultant&rsquo;s MOD Administrator (tenant admin) account. 
  <br><br>Enter your fellow student's tenant admin password in the <strong>Password</strong> field, and then select <strong>OK</strong>.</li>
<li>The commands in lines 41-51 in the script MUST be run individually. If you select all six commands and run them all together at one time, the commands will fail. 
  <br><br>Therefore, at the command prompt, select line <strong>41</strong> in the script and then select the <strong>Run Selection (F8)</strong> icon on the menu bar. <strong>Note:</strong> This command in row 41 creates a new column in the distribution list that does not exist in the Excel spreadsheet. For each record imported from the spreadsheet into this distribution list, the value of this column will be blank. The reason you must run this command is that this specific column is required to successfully import the data and create the distribution list using PowerShell. That being said, when you create new filtered views later on in Task 4, you will ignore this column and not include it in any of the views you create. 
  <br><br>Then select line <strong>43</strong> in the script and select the <strong>Run Selection (F8)</strong> icon on the menu bar.     <br><br>Repeat this process for the commands in lines <strong>45, 47, 49,</strong> and <strong>51</strong>.</li>
<li>At the command prompt, you will run the command in line <strong>60 </strong>by itself; therefore, select this line in the script and then select the <strong>Run Selection (F8)</strong> icon on the menu bar. 
  <br><br><strong>Note: </strong>This command displays the list of sites in the IT Services site. Verify the Service Desk Requests list appears in this list.</li>
<li>At the command prompt, you will run the command in line <strong>66 </strong>by itself; therefore, select this line in the script and then select the <strong>Run Selection (F8)</strong> icon on the menu bar. This command displays all the records in the .csv file that were imported into the terminal.</li>
<li>In the script, lines <strong>73-79</strong> represent one command; therefore, all these lines must be selected together and run as one selection. 
  <br><br>At the command prompt, select lines <strong>73-79</strong> in the script and then select the <strong>Run Selection (F8)</strong> icon on the menu bar. This command will display a summary each of the rows that were imported from the .csv file.</li>
<li>At the command prompt, you have finished running the commands in this script. Close Windows PowerShell.</li>
<li>Open your Edge browser and enter the following URL in the address bar to navigate to the <strong>IT Services</strong> site: <strong>https://xxxxxZZZZZZ.sharepoint.com/sites/ITServices</strong> (where xxxxxZZZZZZ is <u>your tenant prefix</u> provided by your lab hosting provider).</li>
<li>In the <strong>IT Services</strong> site, in the left-hand pane, select <strong>Site contents</strong>. In the list of Site contents, select the <strong>Service Desk Requests</strong> item.</li>
  <li>This displays the <strong>Service Desk Requests</strong> list. Review the 30 items in the list, which should match the 30 items in the .csv file.</li>
<li>Close Windows PowerShell.</li>
<li>Close your Edge browser and proceed to the next task.<br /> </li>
</ol>
<h3>Task 3 - Add Additional Columns to the SharePoint list</h3>
<p>In this task you will return to your role as Holly Dickson. You have just been informed by the IT Consultant that he or she finished exporting the existing ticketing system data and uploaded it to the new SharePoint site. However, as you reviewed the list of data that was imported into the Service Desk Requests list, you noticed that the <strong>Customer</strong> field and the <strong>Assign to</strong> fields were missing. The <strong>Customer</strong> field is the name of the person who entered the ticket, and the <strong>Assign to</strong> field is the name of the support engineer to whom the ticket was assigned. This is critical data for a service request system, so it is imperative that you add this information to the <strong>Service Desk Requests</strong> list.</p>
<ol>
<li>On LON-CL1 you should have closed the Edge browser at the end of the prior task. If not, then do so now. </li>
<li>Since Holly will be using her PC to perform this task, you will use LON-CL1 in this role-playing exercise as Holly&rsquo;s PC rather than the IT Consultant's PC as you did in the prior task.
  <br><br>Select the <strong>Microsoft Edge</strong> icon on the taskbar to open your browser, and then enter the following URL in the address bar: <strong>https://portal.office.com</strong>. </li>
<li>In the <strong>Pick an account</strong> window, select Holly&rsquo;s account if it appears; otherwise, select <strong>Use another account</strong> and then enter <strong>holly@xxxxxZZZZZZ.onmicrosoft.com</strong> (where xxxxxZZZZZZ is the tenant prefix assigned to you by your lab hosting provider). In the <strong>Enter password</strong> window, enter <strong>Pa55w.rd</strong> and select <strong>Sign in</strong>.</li>
<li>After reviewing the data that was imported into the Service Desk Requests list, you noticed that the <strong>Customer</strong> field and the <strong>Assign to</strong> fields were missing. However, after reviewing the spreadsheet, you realized the missing data wasn&rsquo;t an upload issue because the <strong>Customer</strong> and <strong>Assign To</strong> columns were missing from the spreadsheet. 
<br><br>While you cannot explain what caused this, you remember making a backup of the original spreadsheet. If these missing columns are in your backup file, you plan to add the two columns from your backup file to the <strong>Service Desk Requests</strong> list that is displayed in the IT Services site.
<br><br>Select the <strong>File Explorer</strong> icon on the taskbar to return to the <strong>Documents</strong> folder that you opened in the prior task. Double-click on the <strong>Backupfile.xlsx</strong> file to open it.</li>
<li>Review the columns in the table and verify the <strong>Assign to</strong> and <strong>Customer </strong>columns appear. Since you have just verified that this data was captured in your backup file, you can proceed with adding these columns to the <strong>Service Desk Requests</strong> list.</li>
<li>In your Edge browser, in the <strong>Office 365 home </strong>page, select the <strong>SharePoint</strong> icon in the column of Microsoft 365 app icons on the left-side of the screen.
  <br><br>If a <strong>Pick an account</strong> window appears, select Holly's account. </li>
<li>A <strong>News from sites</strong> window appears over top of the SharePoint admin center. Close this window. </li>
<li>On the <strong>SharePoint admin center</strong>, in the left-hand navigation pane, scroll down and under the <strong>Recent</strong> group, select <strong>IT Services</strong>.</li>
<li>On the <strong>IT Services </strong>site, near the bottom of the left-hand navigation pane, select the <strong>X</strong> above <strong>Microsoft Teams</strong> to hide this banner, and in the <strong>Hide </strong>dialog box, select <strong>Yes </strong>to confirm it. 
<br><br>In the left-hand navigation pane, select <strong>Site Contents</strong>, and in the <strong>Contents</strong> list, select <strong>Service Desk Requests</strong>. You want to create a new column to display the <strong>Customer</strong> data that you will import from the <strong>Backupfile.xlsx</strong> spreadsheet.  </li>
<li>On the menu bar at the top of the page, the option to the right of the <strong>+New</strong> button will either display <strong>Edit in grid view</strong> or <strong>Exit grid view</strong>. This option allows you to toggle in or out of grid view. You do NOT want to be in grid view to edit the list. 
<br><br>If this option displays <strong>Edit in grid view</strong>, it means you are not in grid view, so proceed to the next step.   
<br><br>If this option displays <strong>Exit grid view</strong>, then you are currently in grid view, which you do not want to be in. In this case, select <strong>Exit grid view</strong>. </li>
<li>At the end of the column heading row, select <strong>+Add column</strong>, and then in the drop-down menu that appears, select <strong>Person</strong>. </li>
<li>In the <strong>Create a column</strong> window that appears, enter <strong>Customer</strong> in the <strong>Name</strong> field.</li>
<li>In the <strong>Type</strong> field, verify it's already set to <strong>Person or Group</strong>.</li>
<li>Verify the <strong>Allow selection of Groups</strong> check box is NOT selected. Do NOT select this check box. </li>
<li>Select <strong>More options</strong>.</li>
<li>Select the <strong>Require that this column contains information</strong> toggle switch to change it to <strong>Yes</strong>. </li>
<li>Select <strong>Save</strong>.</li>
<li>The <strong>Customer</strong> column should appear in the list. All record entries for this column should be highlighted in yellow and <strong>Required info</strong> should appear in this column for each record (this is because you set the <strong>Require that this column contains information</strong> option to <strong>Yes </strong>in the previous step when you created this column).</li>
<li>Earlier, you were instructed to not be in grid view to add the Customer column. However, now that you have added the column, you must switch to grid view to copy and paste in the Column data from the Backupfile.xlsx spreadsheet. 
  <br><br>On the menu bar, select <strong>Edit in grid view</strong>. In the next few steps, you will copy the Customer data from the <strong>BackupCopy</strong> spreadsheet and paste it into this column in the SharePoint list.</li>
<li>Select the <strong>Excel</strong> spreadsheet icon on the taskbar to display the <strong>BackupFile.xlsx </strong>spreadsheet. Select all the items in the <strong>Customer</strong> column (start in row 2 so that you do not copy the column header), then right-click and select <strong>Copy</strong> from the menu (NOTE: Use the Copy option here instead of <strong>Ctrl+C</strong> to copy the column data; Ctrl+C sometimes results in an error when you attempt to paste in the copied cells in the next step). 
  <br><br><strong>Note:</strong> If a window appears showing the progress of the Copy command, do NOT proceed until the pane disappears. This may take a minute or so for the copy process to complete. If a progress window does not appear, then proceed to the next step.</li>
<li>Select the <strong>Edge</strong> browser icon on the taskbar, which should return you to the grid view page for the <strong>Service Desk Requests</strong> list. Select all the empty fields in the <strong>Customer </strong>column and press <strong>Ctrl+V</strong>. All items will automatically appear in the appropriate row for the<strong> Customer</strong> column.</li>
<li>Select the <strong>Exit grid view</strong> option on the menu bar to see how the Customer data appears in normal display view. 
<li>Repeat steps <strong>11-22</strong> to add a column for the <strong>Assign To</strong> data and to copy the <strong>Assign to</strong> data from the <strong>BackupFile.xlsx</strong> spreadsheet and paste it into the <strong>Service Desk Requests</strong> list.</li>
<li>After reviewing the changes to the <strong>Service Desk Requests</strong> list, you realize that the data type of the <strong>Description</strong> column only supports a <strong>single line of text</strong>. While this is fine for the existing data, going forward you want your customer support engineers to be able to enter more detailed information. Therefore, you want to modify this column to change the data type to <strong>multiple lines of text</strong>. 
  <br><br>To make this change, select the <strong>Description</strong> column heading. In the menu that appears, select <strong>Column Settings</strong>, and then in the sub-menu, select <strong>Edit</strong>.</li>
<li>In the <strong>Edit column</strong> window, select the drop-down arrow in the <strong>Type</strong> field and select <strong>Multiple lines of text</strong>.</li>
<li>Select <strong>More options</strong>.</li>
<li>Change the <strong>Require that this column contains information</strong> option to <strong>Yes</strong>.</li>
<li>Select <strong>Save</strong>.</li>
<li>Leave the browser and all existing tabs open on LON-CL1 for the next task.</li>
</ol>
<h3>Task 4 - Create filtered views for targeted viewing</h3>
<p>In this task, you will continue in your role as Holly Dickson, Adatum&rsquo;s Enterprise Administrator. You were just informed by your IT Consultant that while the default <strong>All items</strong> view in the <strong>Service Desk Requests</strong> list will display all the existing service tickets, this will not help the Customer Support Manager when she wants to focus on specific groups of cases. To address this issue, the IT Consultant has recommended that you create the following new filtered views to provide this visibility:</p>
<ul>
<li>Active cases by Support Agent</li>
<li>Closed cases by Support Agent</li>
<li>All Cases by Support Agent</li>
<li>All Cases by Customer</li>
</ul>
<ol>
<li>You should still be signed into LON-CL1 as the <strong>Administrator</strong>, and you should be logged into Microsoft 365 as Holly Dickson. In your browser, you should still have the tab open from the prior task that displays the <strong>Service Desk Requests</strong> list. If not, then navigate to this list now.</li>
<li>You will begin by creating a view showing all active cases. On the <strong>Service Desk Requests</strong> page, select the <strong>gear</strong> (<strong>Settings</strong>) icon in the top right corner of the webpage. In the menu that appears, select <strong>List settings.</strong></li>
<li>In the<strong> Service Desk Requests &gt; Settings </strong>page, scroll down to the bottom of the page and in the <strong>Views</strong> section, select<strong> Create view.</strong></li>
<li>In the<strong> Settings &gt; View Type </strong>page, select<strong> Standard view.</strong></li>
<li>In the<strong> Settings &gt; Create View </strong>page, enter the following information:
<ul>
<li>View Name: <strong>Active Cases by Support Agent</strong></li>
<li>View Audience: <strong>Create a Public View</strong></li>
<li>In the list of Columns, you must first uncheck all the columns currently selected. Then you MUST select the following columns <strong>in the order they appear below</strong>, which is in ascending <strong>Position from left</strong> sequence. If you select them as you progress from top to bottom in the list on the page, the system will automatically adjust the <strong>Position from left</strong> values to different values:
<ul>
<li><strong>Assign To</strong> &ndash; Position from left: <strong>1</strong></li>
<li><strong>Date</strong> &ndash; Position from left: <strong>2</strong></li>
<li><strong>Customer</strong> &ndash; Position from left: <strong>3</strong></li>
<li><strong>Location</strong> &ndash; Position from left: <strong>4</strong></li>
<li><strong>issueTitle</strong> - Position from left: <strong>5</strong></li>
<li><strong>Description</strong> &ndash; Position from left: <strong>6</strong></li>
</ul>
<li>Sort section - First sort by the column: <strong>Assign to</strong> and <strong>Show items in ascending order</strong></li>
<li>Then sort by the column: <strong>Date</strong> and <strong>Show items in ascending order</strong></li>
<li>Filter section - <strong>Show items only when the following is true</strong> </li>
<li>Show the items when column section &ndash; select <strong>Issue status</strong> column</li>
<li>Operand field &ndash; <strong>Is equal to</strong></li>
<li>Condition field &ndash; enter <strong>Active</strong></li>
</ul>
</li>
<li>Scroll to the bottom of the page and select <strong>OK</strong>.</li>
<li>You will now create a view showing all closed cases. On the <strong>Service Desk Requests</strong> page, select the <strong>gear</strong> (<strong>Settings</strong>) icon in the top right corner of the webpage. In the menu that appears, select <strong>List settings.</strong></li>
<li>In the<strong> Service Desk Requests &gt; Settings </strong>page, scroll down to the <strong>Views</strong> section and select<strong> Create view.</strong></li>
<li>In the<strong> Settings &gt; View Type </strong>page, select<strong> Standard view.</strong></li>
<li>In the<strong> Settings &gt; Create View </strong>page, enter the following information:
<ul>
<li>View Name: <strong>Closed Cases by Support Agent</strong></li>
<li>View Audience: <strong>Create a Public View</strong></li>
<li>In the list of Columns, you must first uncheck all the columns currently selected. Then you MUST select the following columns <strong>in the order they appear below</strong>, which is in ascending <strong>Position from left</strong> sequence. If you select them as you progress from top to bottom in the list on the page, the system will automatically adjust the <strong>Position from left</strong> values to different values:
<ul>
<li><strong>Assign To</strong> &ndash; Position from left: <strong>1</strong></li>
<li><strong>Customer</strong> &ndash; Position from left: <strong>2</strong></li>
<li><strong>Location</strong> &ndash; Position from left: <strong>3</strong></li>
<li><strong>issueTitle</strong> - Position from left: <strong>4</strong></li>
<li><strong>Description</strong> &ndash; Position from left: <strong>5</strong></li>
</ul>
<li>Sort section - First sort by the column: <strong>Assign to</strong> and <strong>Show items in ascending order</strong></li>
<li>Filter section - <strong>Show items only when the following is true</strong> </li>
<li>Show the items when column section &ndash; select <strong>Issue status</strong> column</li>
<li>Operand field &ndash; <strong>Is equal to</strong></li>
<li>Condition field &ndash; enter <strong>Closed</strong></li>
</ul>
</li>  
<li>Scroll to the bottom of the page and select <strong>OK</strong>.</li>
<li>You will now create a view showing all cases for each support agent. On the <strong>Service Desk Requests</strong> page, select the <strong>gear</strong> (<strong>Settings</strong>) icon in the top right corner of the webpage. In the menu that appears, select <strong>List settings.</strong></li>
<li>In the<strong> Service Desk Requests &gt; Settings </strong>page, scroll down to the <strong>Views</strong> section and select<strong> Create view.</strong></li>
<li>In the<strong> Settings &gt; View Type </strong>page, select<strong> Standard view.</strong></li>
<li>In the<strong> Settings &gt; Create View </strong>page, enter the following information:
<ul>
<li>View Name: <strong>All Cases by Support Agent</strong></li>
<li>View Audience: <strong>Create a Public View</strong></li>
<li>In the list of Columns, you must first uncheck all the columns currently selected. Then you MUST select the following columns <strong>in the order they appear below</strong>, which is in ascending <strong>Position from left</strong> sequence. If you select them as you progress from top to bottom in the list on the page, the system will automatically adjust the <strong>Position from left</strong> values to different values:
<ul>
<li><strong>Assign To</strong> &ndash; Position from left: <strong>1</strong></li>
<li><strong>Customer</strong> &ndash; Position from left: <strong>2</strong></li>
<li><strong>issueTitle</strong> - Position from left: <strong>3</strong></li>
<li><strong>Location</strong> &ndash; Position from left: <strong>4</strong></li>
<li><strong>Issue Status</strong> &ndash; Position from left: <strong>5</strong></li>
<li><strong>Description</strong> &ndash; Position from left: <strong>6</strong></li>
</ul>
<li>Sort section - First sort by the column: <strong>Assign to</strong> and <strong>Show items in ascending order</strong></li>
<li>Then sort by the column: <strong>Customer</strong> and <strong>Show items in ascending order</strong></li>
<li>Filter section - <strong>Show all items in this view</strong> </li>
</ul>
</li>    
<li>Scroll to the bottom of the page and select <strong>OK</strong>.</li>
<li>You will finish this task by creating a view showing all cases for each customer. On the <strong>Service Desk Requests</strong> page, select the <strong>gear</strong> (<strong>Settings</strong>) icon in the top right corner of the webpage. In the menu that appears, select <strong>List settings.</strong></li>
<li>In the<strong> Service Desk Requests &gt; Settings </strong>page, scroll down to the <strong>Views</strong> section and select<strong> Create view.</strong></li>
<li>In the<strong> Settings &gt; View Type </strong>page, select<strong> Standard view.</strong></li>
<li>In the<strong> Settings &gt; Create View </strong>page, enter the following information:
<ul>
<li>View Name: <strong>All Cases by Customer</strong></li>
<li>View Audience: <strong>Create a Public View</strong></li>
<li>In the list of Columns, you must first uncheck all the columns currently selected. Then you MUST select the following columns <strong>in the order they appear below</strong>, which is in ascending <strong>Position from left</strong> sequence. If you select them as you progress from top to bottom in the list on the page, the system will automatically adjust the <strong>Position from left</strong> values to different values:
<ul>
<li><strong>Customer</strong> &ndash; Position from left: <strong>1</strong></li>
<li><strong>Date</strong> &ndash; Position from left: <strong>2</strong></li>
<li><strong>Assign To</strong> &ndash; Position from left: <strong>3</strong></li>
<li><strong>issueTitle</strong> - Position from left: <strong>4</strong></li>
<li><strong>Location</strong> &ndash; Position from left: <strong>5</strong></li>
<li><strong>Issue Status</strong> &ndash; Position from left: <strong>6</strong></li>
<li><strong>Description</strong> &ndash; Position from left: <strong>7</strong></li>
</ul>
<li>Sort section - First sort by the column: <strong>Customer</strong> and <strong>Show items in ascending order</strong></li>
<li>Then sort by the column: <strong>Date</strong> and <strong>Show items in ascending order</strong></li>
<li>Filter section - <strong>Show all items in this view</strong> </li>
</ul>
</li>    
<li>Scroll to the bottom of the page and select <strong>OK</strong>.</li>
<li>In your Edge browser, close all tabs EXCEPT for the <strong>Microsoft Office Home</strong> tab and the <strong>Microsoft 365 admin center</strong> tab. </li>
</ol>
<p><strong>&nbsp;</strong></p>
<p><strong>Congratulations! You have completed the building blocks for your new Service Desk Ticketing system. You will add additional functionality to the ticketing system in later labs.</strong></p>
<p><strong>&nbsp;</strong></p>
<h1>Proceed to Lab 3 - Exercise 4</h1>
