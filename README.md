# Production_ready_BPM
Production_ready_BPM is an automated system that takes input form entries processes the data, sends personalized emails, and stores modified documents in 3Ddrive and Bookmark Editor.

## Features
- Form submission with User ID, Name, College, Semester, and file upload.
- Sends personalized emails with modified template files.
- Uploads files to cloud storage (3D Drive).
- Uploads documents to the document management system and adds them to the bookmark editor for quick access.

## Pre-requisites

- Access to DS India Cloud Tenant:  
   - The external link to access **DS India Cloud**:  
      [DS India Cloud Access](https://r1132100693975-indw2-ifwe.3dexperience.3ds.com/#dashboard:3e685cbb-2d29-4182-8b59-a799fe7a4f98/tabId:A8o176KA09QJjqNChWTS/fullscreen:A8ZcDT0A09_a7sN84WEG)  
   - Create your own account using your **email ID and password**.  

- Access to the following roles on the platform:  
   - **Business Process Designer** role  
   - **Business Process Play** role  
   - **Bookmark Editor**  
   - **3DDrive**  
   - **3DPlay**  

- Access to the following Security Context:  
   - **VPLMProjectLeader.Company Name.Common Space**  


## Importing the Model

1. Open your **Business Process Designer**.  
2. Locate the **Models** icon on the left-hand side.  
3. Click on **"Import Model"**.  
4. Upload the **Iterop format** model from the repository.  

## Validating and Configuring the Model

1. After importing, locate the **"Validate and Configure"** option in the top left corner.  
2. Click on it to complete the setup.  

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

1. Click on **"Update the Document in 3D Drive"** service task.  
2. Click on **"Choose the Data"**.  
3. Under the **User** field, click **Settings**.  
4. Select the **user** as the creator of the document and click **OK**.  
5. Under the **File** field, ensure the correct file is selected (pre-filled).  
6. Under the **Folder ID** field, click **Settings**.  
7. To get the **Folder ID**:  
   - Click the **arrow** next to the folder name.  
   - Select **"Copy Link"**.  
   - Locate the **"Content ID"**—this is your Folder ID.  
8. Click **OK** to save the changes.

## Updating the Bookmark 

*Bookmarks* in 3DEXPERIENCE allow users to organize and manage important documents and files for easy access and collaboration within the platform.  

1. Click on **"Update in Bookmark"** service task.  
2. Click on **"Choose the Data"**.  
3. Select the **"Bookmark ID"** field and click on **"Settings"** under it.  
4. **Enter the Bookmark ID according to your bookmark.**  
   - If you already have the **Bookmark ID**, enter it directly.  
   - If you do not have the **Bookmark ID**, right-click on the bookmark, **copy the link**, and extract the Bookmark ID by decrypting the encrypted URL.  
5. Under the **"Content Type"** field, click **"Settings"** and set the **name of the file** to be added to your bookmark.  
6. Under the **"User"** field, click **"Settings"**.  
7. Select the **user** to be the **creator** of the document.  
8. Click **OK** to save the changes.  

**Note:**  Ensure that the **Bookmark ID** matches your intended folder in the platform to avoid misplacement of files.  


## Testing

To ensure that your business process works correctly:

- Click on the **Test** icon.  
- Under **Scripts and Service Tasks**, select **Execute Normally** and press **OK**.  
- In the pop-up window, click **Start this test process from Play** to begin the test.  
- Fill in all **mandatory fields** and press **Start**.  
- Navigate to the **Monitoring** section on the **left-hand side**.  
- Select your process **"Production_ready_Bpm"** under the **Finished** tab.  
- **Check for Errors:**  
   - ✅ If no errors are found, your process has been successfully tested.  
   - ❌ If errors are detected, review and fix them in your business process design.  
- Re-run the test after making corrections until the process is error-free.

  
## Deployment

To deploy the model successfully:

1. Open **Business Process Designer**.  
2. Select the process **"Production_ready_model"**.  
3. Click on **"Deploy Model"** to publish the process.  

✅ Once deployed, the model is ready to be used for executing tasks like adding entries, sending emails, and uploading documents.  

## Customizing Model Settings

Before deployment, configure the following settings to ensure easy identification and smooth management:

- **Priority:** Set the priority of the process to categorize tasks based on urgency.  
   - Default: **Normal**, but you can change it to **Low, High**, or **Critical** depending on your business needs.  

- **Process Color:** Assign a **color** to the process to differentiate it visually from other models.  
   - Choose a color that reflects the importance or category of the process.  

- **Tags:** Add relevant **tags** (e.g., "intern") to quickly locate and categorize the model.  
   - Tags make it easier to filter and identify processes in the repository.  

## Changing Ownership

If you need to transfer ownership:

1. Click on **"Change Owner"**.  
2. Select the new owner from the list of available users.  
3. Click **OK** to confirm the ownership change.  

Ownership change ensures that the right person has control over the model and its configurations.  

## Modifying Role Assignments

After deployment, configure user roles to control process access and monitoring:

- **Initiators:** Define who can **start the process**.  
   - You can allow **external access** or restrict it to specific users.  

- **Supervisors and Limited Supervisors:** Assign supervisors to **monitor and manage** the process.  
   - Supervisors can have limited access or full monitoring rights, depending on your configuration.  

- **Controllers:** Handle **error notifications** and monitor unexpected behavior.  
   - Assign a controller to oversee critical tasks and resolve issues efficiently.  

- **Choose Roles:**  
   1. Click on **"Choose Roles"**.  
   2. Select the required roles (supervisors/controllers).  
   3. Click **OK** to save the changes.  

- **Visibility Settings:** Toggle **"Diagram visible to all users"** to control who can view the process diagram.  



