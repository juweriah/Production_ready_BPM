# Production_ready_BPM  
Production_ready_BPM is an automated system that takes input from form entries, processes the data, sends personalized emails, and stores modified documents in 3D Drive and Bookmark Editor.

## Features  

- Form submission with **User ID**, **Name**, **College**, **Semester**, and **Email ID**.  
- Sends personalized emails with modified template files.  
- Uploads files to cloud storage (3D Drive).  
- Uploads documents to the document management system and adds them to the Bookmark Editor for quick access.  

## Pre-requisites  

- Access to Cloud Tenant:  

- Access to the following roles on the platform:  
   - **Business Process Designer** role  
   - **Business Process Play** role    

## Importing the Model  

- Open your **Business Process Designer**.  
- Locate the **Models** icon on the left-hand side.  
- Click on **"Import Model"**.  
- Upload the **Iterop format** model from the repository.  

## Validating and Configuring the Model  

- After importing, locate the **"Validate and Configure"** option in the top left corner.  
- Click on it to complete the setup.  

## Business Table (InternData)  

- The first process involves **adding data** to the business table.  
- The uploaded file is **cloned and converted** into a PDF document.  
- The business table (**InternData**) is pre-created and automatically stores new entries.  

## Sending an Email  

- The email contains the following **pre-filled fields**:  
   - Recipient Email  
   - Subject  
   - Message  
   - Attachments (if needed)  
   - Other required fields based on your preferences  

- Modify any of these fields as needed to suit your requirements.  

## Updating a Document in 3D Drive  

- Click on **"Update the Document in 3D Drive"** service task.  
- Click on **"Choose the Data"**.  
- Under the **User** field, click **Settings**.  
- Select the **user** as the creator of the document and click **OK**.  
- Under the **File** field, ensure the correct file is selected (pre-filled).  
- Under the **Folder ID** field, click **Settings**.  
- To get the **Folder ID**:  
   - Click the **arrow** next to the folder name.  
   - Select **"Copy Link"**.  
   - Locate the **"Content ID"**—this is your Folder ID.  
- Click **OK** to save the changes.  

## Updating the File in Document  

- Click on **"Update the Cloned File in Document"** service task.  
- Click on **"Choose the Data"**.  
- Select the **"Title"** field and click on **"Settings"** under it.  
- Set the **file name** according to user requirements and click **OK**.  
- Under the **"User"** field, click **"Settings"**.  
- Select the **user** to be the **creator** of the document.  
- Click **OK** to save the changes.  

- **Note:** The **Security Context** must be set according to **responsibility rights** as stated in the **Pre-requisites** section to ensure proper access control.  

## Updating the Bookmark  

- Click on **"Update in Bookmark"** service task.  
- Click on **"Choose the Data"**.  
- Select the **"Bookmark ID"** field and click on **"Settings"** under it.  
- **Enter the Bookmark ID according to your bookmark.**  
   - If you already have the **Bookmark ID**, enter it directly.  
   - If you do not have the **Bookmark ID**, right-click on the bookmark, **copy the link**, and extract the Bookmark ID by decrypting the encrypted URL.  
- Under the **"Content Type"** field, click **"Settings"** and set the **name of the file** to be added to your bookmark.  
- Under the **"User"** field, click **"Settings"**.  
- Select the **user** to be the **creator** of the document.  
- Click **OK** to save the changes.  

- **Note:** Ensure that the **Bookmark ID** matches your intended folder in the platform to avoid misplacement of files.  

## Testing  

- Click on the **Test** icon.  
- Under **Scripts and Service Tasks**, select **Execute Normally** and press **OK**.  
- In the pop-up window, click **"Start this test process from Play"** to begin the test.  
- Fill in all **mandatory fields** and press **Start**.  
- Navigate to the **Monitoring** section on the **left-hand side**.  
- Select your process **"Production_ready_BPM"** under the **Finished** tab.  
- **Check for Errors:**  
   - ✅ If no errors are found, your process has been successfully tested.  
   - ❌ If errors are detected, review and fix them in your business process design.  
- Re-run the test after making corrections until the process is error-free.  

## Deployment  

- Open **Business Process Designer**.  
- Select the process **"Production_ready_model"**.  
- Click on **"Deploy Model"** to publish the process.  

### Customizing Model Settings  

- **Priority:** Set the priority of the process to categorize tasks based on urgency.  
   - Default: **Normal**, but you can change it to **Low, High**, or **Critical** depending on your business needs.  
- **Process Color:** Assign a **color** to the process to differentiate it visually from other models.  
- **Tags:** Add relevant **tags** (e.g., "intern") to quickly locate and categorize the model.  

### Changing Ownership  

- Click on **"Change Owner"**.  
- Select the new owner from the list of available users.  
- Click **OK** to confirm the ownership change.  

### Modifying Role Assignments  

- **Initiators:** Define who can **start the process**.  
- **Supervisors and Limited Supervisors:** Assign supervisors to **monitor and manage** the process.  
- **Controllers:** Handle **error notifications** and monitor unexpected behavior.  
- **Choose Roles:**  
   - Click on **"Choose Roles"**.  
   - Select the required roles (supervisors/controllers).  
   - Click **OK** to save the changes.  
- **Visibility Settings:** Toggle **"Diagram visible to all users"** to control who can view the process diagram.  



